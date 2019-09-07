# Offcie 2019 安装

office 和visio只能同版本无法共存。  
因此同时下载最新的2019安装。尝试多次无法成功。  
始终报错30175-11，google到两种方案。  
 1. 修改C:\ProgramData\Microsoft\Windows\Start Menu\Programs
 2. 使用微软专用工具卸载后重装。  

两种方案均尝试无果。后来发现C:\ProgramData\Microsoft\Windows\Start Menu\Programs
文件夹为只读模式。尝试修改后安装成功。

[:back:返回主目录](../README.md)
