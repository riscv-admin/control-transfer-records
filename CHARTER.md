# Control Transfer History Task Group Charter

Profile-guided optimization tools, such as autofdo, depend on accurate instruction profiles to guide compilation and effect performance improvements.  Research has demonstrated that collecting recent control transfer history with each sampled program counter value results in richer, more accurate profiles that greatly improve optimization results.

The Control Transfer History Task Group shall develop a RISC-V control transfer recording specification that enables recording recent transfer history to on-chip storage.  This mechanism will be controlled by privileged software, or a debugger, and will include support for filtering transfer recording by privilege mode.  For each transfer recorded, the source and target address will be recorded, as well as optional metadata.

The specification will be validated by prototyping the extension on QEMU and/or FPGA, with Linux perf.