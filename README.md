# Vm2Import
fix vmprotect import function used unicorn-engine.

it can repair functions such as <code>call [module.function]</code> or <code>jmp [module.function]</code> or <code>reg(mov) [module.function]</code> that are statically imported by the VM.

it is effective in vmp2 and vmp3.

### Use
1. copy to x64dbg
  <code>
  x64dbg\release\x32\plugins\unicorn.dll
  
  x64dbg\release\x32\plugins\Vm2Import.dp32
  </code>
  
  <code>
  x64dbg\release\x64\plugins\unicorn.dll
  
  x64dbg\release\x64\plugins\Vm2Import.dp64
  </code>

2. select "VM_Start" <code>call vmp0.xxxxxxxx</code>, right click menu <code>"Vm2Import"->"Fix Import Call Address"</code>

![repair menu preview](https://i.imgur.com/lMv7MoS.jpg)

3. repair.

![repair preview](https://i.imgur.com/OHGDRXc.jpg)


### original sample:
![original preview](https://i.imgur.com/qwpyNM3.jpg)


### Thanks
- [unicorn](https://github.com/unicorn-engine/unicorn)
- [fmtlib](https://github.com/fmtlib/fmt)
