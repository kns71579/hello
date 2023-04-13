# To RUN this "Hello World" example Python script on Windows 10 using Renode

1) Download and run the renode_1.13.3.msi installer for Renode onto a PC running Windows 10
2) Append C:\Program Files\Renode to the System variables PATH in the Environment Variables
3) Copy the hello.py file from this repository (kns71579/hello) into C:\Program Files\Renode directory
4) Run Renode from the Windows Start menu
   The Renode LOG window and the Renode COMMAND window both open
5) At the (monitor) prompt in the Renode COMMAND window type the command:
   (monitor) mach create
6) At the (machine-0) prompt type the following three commands:
   (machine-0) machine LoadPlatformDescription @platforms/cpus/nRF32840.repl
   (machine-0) start
   (machine-0) include @hello.py
   
