role :hadoop_all, "root@10.15.22.11", "root@10.15.22.12", "root@10.15.22.13", "root@10.15.22.14", "root@10.15.22.15", "root@10.15.22.16", "root@10.15.22.17", "root@10.15.22.18", "root@10.15.22.19", "root@10.15.22.20", "root@10.15.22.21", "root@10.15.22.22", "root@10.15.22.23", "root@10.15.22.24", "root@10.15.22.25", "root@10.15.22.26", "root@10.15.22.27", "root@10.15.22.28", "root@10.15.22.29", "root@10.15.22.31", "root@10.15.22.32", "root@10.15.22.34", "root@10.15.22.35", "root@10.15.22.36", "root@10.15.22.37", "root@10.15.22.38", "root@10.15.22.39", "root@10.15.22.40", "root@10.15.22.41" 
role :hadoop_all2, "10.15.22.11", "10.15.22.12", "10.15.22.13", "10.15.22.14", "10.15.22.15", "10.15.22.16", "10.15.22.17", "10.15.22.18", "10.15.22.19", "10.15.22.20", "10.15.22.21", "10.15.22.22", "10.15.22.23", "10.15.22.24", "10.15.22.25", "10.15.22.26", "10.15.22.27", "10.15.22.28", "10.15.22.29", "10.15.22.31", "10.15.22.32", "10.15.22.34", "10.15.22.35", "10.15.22.36", "10.15.22.37", "10.15.22.38", "10.15.22.39", "10.15.22.40", "10.15.22.41" 

desc "Show Block Devices"
task :show_lsblk, :roles => :hadoop_all do
  run "lsblk"
end
desc "Show Date"
task :show_date, :roles => :hadoop_all do
  run "date"
end
desc "Show Uptime"
task :show_uptime, :roles => :hadoop_all do
  run "uptime"
end
desc "Show Freespace"
task :show_freespace, :roles => :hadoop_all do
  run "df -h /"
end
desc "Show Services"
task :show_services, :roles => :hadoop_all do
  run "netstat -tunpl"
end
desc "Flush Firewall"
task :flush_fw, :roles => :hadoop_all do
  run "iptables -F"
end
desc "Save Firewall"
task :save_fw, :roles => :hadoop_all do
  run "service iptables save"
end
desc "Stop Firewall"
task :stop_fw, :roles => :hadoop_all do
  run "service iptables stop"
end
desc "Firewall Status"
task :stat_fw, :roles => :hadoop_all do
  run "service iptables status"
end
desc "Disable Firewall"
task :disable_fw, :roles => :hadoop_all do
  run "chkconfig iptables off"
end
