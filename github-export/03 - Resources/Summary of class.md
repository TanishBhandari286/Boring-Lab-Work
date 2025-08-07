### 1st lab of Mahesh sir summary

# Windows Internal Processes and Their Specialities

## ntoskrnl.exe (“Windows NT Operating System Kernel Executable”)
- **What it is:** The main Windows **kernel image**.  
- **Speciality:** Core of the Windows OS; contains the kernel and executive services.  
- **Functions:**  
  - Hardware abstraction (via HAL)  
  - Memory management  
  - Process/thread scheduling  
  - Interrupt handling  
  - Security enforcement (reference monitor)  
  - System crash handling ("blue screen of death")

## smss.exe (Session Manager Subsystem)
- **What it is:** The very first user-mode process created during system boot.  
- **Speciality:** Starts system sessions and launches critical processes like `csrss.exe` and `wininit.exe`.  
- **Functions:**  
  - Initializes environment for user sessions  
  - Creates user-mode subsystems  
  - Starts `csrss.exe`, `wininit.exe` and cleans up sessions

## csrss.exe (Client/Server Runtime Subsystem)
- **What it is:** User-mode system process managing console windows and process/thread creation.  
- **Speciality:** Acts as a bridge between user-mode APIs and kernel.  
- **Functions:**  
  - Manages Win32 API calls  
  - Controls console and graphical related events  
  - Handles process/thread creation and shutdown tasks

## wininit.exe (Windows Initialization Process)
- **What it is:** Process started during boot for session 0 initialization.  
- **Speciality:** Orchestrates starting of system services and critical processes.  
- **Functions:**  
  - Starts `services.exe` (Service Control Manager)  
  - Starts `lsass.exe` (Local Security Authority Subsystem)  
  - Starts `lsm.exe` (Local Session Manager)  

## services.exe (Service Control Manager - SCM)
- **What it is:** Manages all Windows services.  
- **Speciality:** Controls starting, stopping, and lifecycle of background services and drivers.  
- **Functions:**  
  - Loads and manages system services  



---

### Summary Table

| Process      | Unique Role / Speciality                                            |
| ------------ | ------------------------------------------------------------------- |
| ntoskrnl.exe | Core kernel: hardware, memory, processes, interrupts management     |
| smss.exe     | Session manager: bootstraps user-mode and system-critical processes |
| csrss.exe    | Manages console, threads, and Win32 API bridge                      |
| wininit.exe  | Initializes system services and session 0 processes                 |


