# preemptive-task-scheduler-for-lua

Problem we are trying to solve is that when running a long .lua scrpt function it will block the main thread. This often a problem in realtime systems like game engines. This code will intterupt the lua interpreter using lua_hook that for given instruction count and give the control back to the calling thread. Then again calling the call_function_non_blocking() will resume the lua function execution from last intterupted point of the code.

# Build information
Please dowbload lua c-api from https://www.lua.org/download.html
There is no make or cmake script for building this project. Just copy Preemptive_lua_test.c to visual studio or compile with your favorite compiler. 

# Running 
Place non_blocking_test.lua in the workspace.


