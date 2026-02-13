1.adb命令，这个命令会启动一个 20 秒钟的跟踪，收集指定的数据源信息，并将跟踪文件保存到 /data/misc/perfetto-traces/trace_file.perfetto-trace
adb shell perfetto -o /data/misc/perfetto-traces/trace_file.perfetto-trace -t 20s \sched freq idle am wm gfx view binder_driver hal dalvik camera input res memory
文件pull出来
adb pull /data/misc/perfetto-traces/trace_file.perfetto-trace