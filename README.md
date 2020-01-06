# log-serial0
- Script to log Raspberry Pi UART /dev/serial0 at 115200 baud
- Will create directory `~/log` and place log files there
- Will create log files named with date and time: `05Jan20-17:48:08.log`
- Log file will be closed at 1000 lines, and then a new file created
- Ensure user is member of dialout group: `sudo usermod -aG dialout user`
- Don't forget to `chmod +x ./log-serial0`
- Run with `nohup ./log-serial0 &`
