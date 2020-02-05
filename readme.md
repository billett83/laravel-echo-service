# Laravel-echo-server systemd Service

Implement this file into systemd to run Laravel-echo-server as a service as an alternative option to using Supervisord

## Installation

Edit hte service file updating the `WorkingDirectory` to match that patch of your Laravel-echo-server .conf file

#### RedHat/Centos/AWSLinux

```bash
cp laravel-echo-server.service /lib/init.d/system/<new service name>.service
```

#### Ubuntu/Debian

```bash
cp laravel-echo-server.service /etc/system.d/system/<new service name>.service
```

## Running the service

```bash
systemctl start <new service name>
```

