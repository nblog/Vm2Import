# Vm2Import
fix vmprotect import function used unicorn-engine.
- `call/jmp/reg(mov) [module.function]`
- work in vmp2.x ~ vmp3.6

### Use
- command: `vm2iat dis.sel()`
- `call vmp0.xxxxxxxx`, right click `"Vm2Import"->"Fix Import Call Address"`

![repair menu preview](https://i.imgur.com/lMv7MoS.jpg)

![repair preview](https://i.imgur.com/OHGDRXc.jpg)

![original preview](https://i.imgur.com/qwpyNM3.jpg)


### Thanks
- [unicorn](https://github.com/unicorn-engine/unicorn)
- [fmtlib](https://github.com/fmtlib/fmt)
- [spdlog](https://github.com/gabime/spdlog)