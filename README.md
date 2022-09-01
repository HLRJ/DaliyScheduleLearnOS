# DaliyScheduleLearnOS
记录学习rCore

## Day01
我大概有点小基础，就直接去做小练习了  

配置Github Classroom模式的Rustling小练习，在 `sudo make codespaces_setenv`  后并没有正常执行完全，
大概是这个样子:  
`To get started you may need to restart your current shell.`  
`This would reload your PATH environment variable to include`  
`Cargo's bin directory ($HOME/.cargo/bin).`

`To configure your current shell, run:`  
`source "$HOME/.cargo/env"`  
`/bin/zsh && source /home/codespace/.cargo/env`

需手动在终端输入
`source "$HOME/.cargo/env"
/bin/zsh && source /home/codespace/.cargo/env`  
以及  
`cargo install --force --path .`  
此时再输入 `rustlings` 即可出现测验信息。  
