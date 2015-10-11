# openaps-notes

Th Sep 24 2015 13:59:13

```
20150920_254pm       20150924_1133pm  20150925_154am  openaps.ini
20150920_805pm       20150924_1150pm  20150929_853am  openaps-monitor
20150920_952pm       20150924_159pm   bin             python_games
20150923_213pm_real  20150924_536pm   myopenaps       typescript
20150923_311pm       20150924_611pm   openaps-dose
pi@cgmcloud1 ~ $ cat 20150924_159pm
Script started on Thu 24 Sep 2015 13:59:13 PDT
pi@raspberrypi ~ $ ls
20150920_254pm  20150920_952pm  20150924_159pm  openaps.ini   typescript
20150920_805pm  20150923_311pm  myopenaps       python_games
pi@raspberrypi ~ $ cd ..
pi@raspberrypi /home $ ls
pi
pi@raspberrypi /home $ cd ..
pi@raspberrypi / $ ls
bin   dev  home  lost+found  mnt  proc  run   selinux  sys  usr
boot  etc  lib   media       opt  root  sbin  srv      tmp  var
pi@raspberrypi / $ cd etc
pi@raspberrypi /etc $ ls
adduser.conf            init             ppp
alternatives            init.d           profile
apm                     initramfs-tools  profile.d
apparmor.d              inittab          protocols
apt                     inputrc          pulse
avahi                   insserv          python
bash.bashrc             insserv.conf     python2.7
bash_completion         insserv.conf.d   python3
bash_completion.d       iproute2         python3.2
bindresvport.blacklist  issue            rc0.d
ca-certificates         issue.net        rc1.d
ca-certificates.conf    issue.net.orig   rc2.d
calendar                issue.orig       rc3.d
ConsoleKit              kbd              rc4.d
console-setup           kernel           rc5.d
cron.d                  ldap             rc6.d
cron.daily              ld.so.cache      rc.local
cron.hourly             ld.so.conf       rcS.d
cron.monthly            ld.so.conf.d     request-key.d
crontab                 ld.so.preload    resolvconf
cron.weekly             libaudit.conf    resolv.conf
dbus-1                  libnl-3          resolvconf.conf
debconf.conf            libpaper.d       rmt
debian_version          lightdm          rpc
default                 locale.alias     rpi-issue
deluser.conf            locale.gen       rsyslog.conf
dhcp                    localtime        rsyslog.d
dhcp3                   logcheck         samba
dhcpcd.conf             login.defs       securetty
dhcpcd.duid             logrotate.conf   security
dictionaries-common     logrotate.d      selinux
dillo                   magic            services
dphys-swapfile          magic.mime       sgml
dpkg                    mailcap          shadow
drirc                   mailcap.order    shadow-
emacs                   manpath.config   shells
environment             menu             skel
esound                  menu-methods     ssh
fake-hwclock.data       mime.types       ssl
fb.modes                mke2fs.conf      staff-group-for-usr-local
fonts                   modprobe.d       sudoers
fstab                   modules          sudoers.d
fstab.d                 motd             sysctl.conf
fuse.conf               motd.tail        sysctl.d
gai.conf                mtab             systemd
gconf                   nanorc           terminfo
gdb                     netconfig        timezone
ghostscript             network          timidity
gnome                   networks         triggerhappy
groff                   nsswitch.conf    ts.conf
group                   ntp.conf         ucf.conf
group-                  openal           udev
gshadow                 opt              ufw
gshadow-                os-release       vim
gssapi_mech.conf        os-release.orig  watchdog.conf
gtk-2.0                 pam.conf         weston
gtk-3.0                 pam.d            wgetrc
host.conf               papersize        wildmidi
hostname                passwd           wpa_supplicant
hosts                   passwd-          X11
hosts.allow             perl             xdg
hosts.deny              plymouth         xml
idmapd.conf             pm               xpdf
ifplugd                 polkit-1
pi@raspberrypi /etc $ cd network/
pi@raspberrypi /etc/network $ ls
if-down.d       if-pre-up.d  interfaces           interfaces.save
if-post-down.d  if-up.d      interfaces.dpkg-old  run
pi@raspberrypi /etc/network $ sudo nano interfaces
```

Th 24 Sep 2015 14:13:10 

```
Script started on Thu 24 Sep 2015 14:13:10 PDT
^[]0;pi@raspberrypi: ~^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~ $^[[00m cd myopenaps/
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m opean^H^[[K^H^[[Knaps use pump -h
usage: openaps-use pump [-h] USAGE ...

optional arguments:
  -h, --help            show this help message and exit

## Device pump:
  vendor openaps.vendors.medtronic

  Medtronic - openaps driver for Medtronic



  USAGE                 Usage Details
    Session             session for pump
    bolus               Send bolus.
    filter_glucose_date
                        Search for glucose pages including begin and end dates
                        (iso 8601).
    filter_isig_date    Search for isig pages including begin and end dates
                        (iso 8601).
    iter_glucose        Read latest 100 glucose records
    iter_glucose_hours  Read latest n hours of glucose data
    iter_pump           Read latest 100 pump records
    iter_pump_hours     Read latest n hours of pump records
    model               Get model number
    mytest              Testing read_settings
    read_basal_profile_A
                        Read basal profile A.
    read_basal_profile_B
                        Read basal profile B.
    read_basal_profile_std
                        Read default basal profile.
    read_battery_status
                        Check battery status.
    read_bg_targets     Read bg targets.
    read_carb_ratios    Read carb_ratios.
    read_clock          Read date/time of pump
    read_current_glucose_pages
                        Read current glucose pages.
    read_current_history_pages
                        Read current history pages.
    read_glucose_data   Read pump glucose page
    read_history_data   Read pump history page
    read_insulin_sensitivies
                        Read insulin sensitivies.
    read_selected_basal_profile
                        Fetch the currently selected basal profile.
    read_settings       Read settings.
    read_status         Get pump status
    read_temp_basal     Read temporary basal rates.
    reservoir           Get pump remaining insulin
    resume_pump         resume pumping.
    scan                scan for usb stick
    set_temp_basal      Set temporary basal rates.
    settings            Get pump settings
    status              Get pump status (alias for read_status)
    suspend_pump        Suspend pumping.
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m ^M^[[K^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[0$
Traceback (most recent call last):
  File "/usr/local/bin/openaps-use", line 5, in <module>
    pkg_resources.run_script('openaps==0.0.6', 'openaps-use')
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 499, in run_script
    self.require(requires)[0].run_script(script_name, ns)
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 1235, in run_script
    execfile(script_filename, namespace, namespace)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-use", line 63, in <module>
    app( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 44, in __call__
    self.run(self.args)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-use", line 57, in run
    output = app(args, self)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/__init__.py", line 92, in __call__
    return self.method.selected(args)(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/__init__.py", line 31, in __call__
    return self.method(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/use.py", line 26, in __call__
    output = self.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/vendors/medtronic.py", line 193, in main
    return getattr(self.pump.model, name)(**self.get_params(args))
AttributeError: 'Model522' object has no attribute 'read_basal_profile_B'
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps use pump read_basal_profile_B^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^$
[
  {
    "i": 0,
    "start": "00:00:00",
    "rate": 0.6000000000000001,
    "minutes": 0
  },
  {
    "i": 1,
    "start": "03:00:00",
    "rate": 0.8,
    "minutes": 180
  },
  {
    "i": 2,

    "start": "05:00:00",
    "rate": 0.8,
    "minutes": 300
  },
  {
    "i": 3,
    "start": "07:00:00",
    "rate": 1.25,
    "minutes": 420
  },
  {
    "i": 4,
    "start": "11:00:00",
    "rate": 1.0,
    "minutes": 660
  },
  {
    "i": 5,
    "start": "12:00:00",
    "rate": 0.7000000000000001,
    "minutes": 720
  },
  {
    "i": 6,
    "start": "17:00:00",
    "rate": 0.65,
    "minutes": 1020
  },
  {
    "i": 7,
    "start": "20:00:00",
    "rate": 0.9,
    "minutes": 1200
  },
  {
    "i": 8,
    "start": "22:00:00",
    "rate": 0.9,
    "minutes": 1320
  }
]^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openap ^H^[[Ks use pump^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^H$
Traceback (most recent call last):
  File "/usr/local/bin/openaps", line 5, in <module>
    pkg_resources.run_script('openaps==0.0.6', 'openaps')
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 499, in run_script
    self.require(requires)[0].run_script(script_name, ns)
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 1235, in run_script
    execfile(script_filename, namespace, namespace)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps", line 158, in <module>
    app( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 44, in __call__
    self.run(self.args)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps", line 152, in run
    exit(call(['openaps-%s' % args.command ] + args.args))
  File "/usr/lib/python2.7/subprocess.py", line 493, in call
    return Popen(*popenargs, **kwargs).wait()
  File "/usr/lib/python2.7/subprocess.py", line 679, in __init__
    errread, errwrite)
  File "/usr/lib/python2.7/subprocess.py", line 1259, in _execute_child
    raise child_exception
OSError: [Errno 2] No such file or directory
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps pum^H^[[K^H^[[K^H^[[Kpurple^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^H^[[Kuse$
added medtronic://purple
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m opeanps use pump -h
bash: opeanps: command not found
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m opeanps use pump -h^H^H^H^H^H^H^H^H^H^H^H^H^H^H^H^[[1P^H^[[1P^[[1@n^[[1@a
usage: openaps-use pump [-h] USAGE ...

optional arguments:
  -h, --help            show this help message and exit

## Device pump:
  vendor openaps.vendors.medtronic

  Medtronic - openaps driver for Medtronic



  USAGE                 Usage Details
    Session             session for pump
    bolus               Send bolus.
    filter_glucose_date
                        Search for glucose pages including begin and end dates
                        (iso 8601).
    filter_isig_date    Search for isig pages including begin and end dates
                        (iso 8601).
    iter_glucose        Read latest 100 glucose records
    iter_glucose_hours  Read latest n hours of glucose data
    iter_pump           Read latest 100 pump records
    iter_pump_hours     Read latest n hours of pump records
    model               Get model number
    mytest              Testing read_settings
    read_basal_profile_A
                        Read basal profile A.
    read_basal_profile_B
                        Read basal profile B.
    read_basal_profile_std
                        Read default basal profile.
    read_battery_status
                        Check battery status.
     read_bg_targets     Read bg targets.
    read_carb_ratios    Read carb_ratios.
    read_clock          Read date/time of pump
    read_current_glucose_pages
                        Read current glucose pages.
    read_current_history_pages
                        Read current history pages.
    read_glucose_data   Read pump glucose page
    read_history_data   Read pump history page
    read_insulin_sensitivies
                        Read insulin sensitivies.
    read_selected_basal_profile
                        Fetch the currently selected basal profile.
    read_settings       Read settings.
    read_status         Get pump status
    read_temp_basal     Read temporary basal rates.
    reservoir           Get pump remaining insulin
    resume_pump         resume pumping.
    scan                scan for usb stick
    set_temp_basal      Set temporary basal rates.
    settings            Get pump settings
    status              Get pump status (alias for read_status)
    suspend_pump        Suspend pumping.
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps use pm^H^[[Kump read_^H^[[K^H^[[K^H^[[K^H^[[K^H$
"523"^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps use purple model^H^[[K^H^[[K^H^[[K^H^[[K^H$
{
  "status": "normal",
  "bolusing": false,
  "suspended": false
}^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps use purple read_basal_profile^H^[[K^H^[[K^H^[[$
{
  "status": "suspended",
  "recieved": true,
  "enacted_at": "2015-09-24T14:46:10.650519"
}^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m opean^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^G^V^X
bash: $'\026\030': command not found
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m ^M^[[K^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@ras$

{
  "temp": "absolute",
  "recieved": true,
  "rate": 1.5,
  "timestamp": "2015-09-24T14:49:44.998115",
  "duration": 30
}^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m {
>   "requested": {
> {   "requested": {^M^[[C^[[Cecho '{"rate": 1.5, "duration": 30, "temp": "absolute"}' | openaps use pump set_temp_basal -^H^H^H^H^H^H^H^H^H^H^H^H^H$
> ^C
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m echo '{"rate": 1.5, "duration": 30, "temp": "absolute"}$
^[[D^[[D^[[B^CTraceback (most recent call last):
  File "/usr/local/bin/openaps", line 5, in <module>
    pkg_resources.run_script('openaps==0.0.6', 'openaps')
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 499, in run_script
    self.require(requires)[0].run_script(script_name, ns)
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 1235, in run_script
    execfile(script_filename, namespace, namespace)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps", line 158, in <module>
    Traceback (most recent call last):
  File "/usr/local/bin/openaps-use", line 5, in <module>
    pkg_resources.run_script('openaps==0.0.6', 'openaps-use')
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 499, in run_script
    self.require(requires)[0].run_script(script_name, ns)
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 1235, in run_script
    execfile(script_filename, namespace, namespace)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-use", line 63, in <module>
    app( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 44, in __call__
    self.run(self.args)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-use", line 57, in run
    output = app(args, self)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/__init__.py", line 92, in __call__
    return self.method.selected(args)(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/__init__.py", line 31, in __call__
    return self.method(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/use.py", line 26, in __call__
    output = self.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/vendors/medtronic.py", line 279, in main
    results = self.upload_program(program)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/vendors/medtronic.py", line 288, in upload_program
    return self.pump.model.set_temp_basal(**program)
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/models/__init__.py", line 182, in set_temp_basal
app( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 44, in __call__
    self.run(self.args)
    result = self._set_temp_basal(**basals)
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/models/__init__.py", line 22, in __call__
    self.response = inst.session.query(self.msg, **kwds)
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/session.py", line 110, in query
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps", line 152, in run
    exit(call(['openaps-%s' % args.command ] + args.args))
    self.execute(command)
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/session.py", line 107, in execute
    return super(type(self), self).execute(command)
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/session.py", line 39, in execute
    self.download( )
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/session.py", line 52, in download
    data = self.stick.download( )
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/stick.py", line 730, in download
  File "/usr/lib/python2.7/subprocess.py", line 493, in call
    return Popen(*popenargs, **kwargs).wait()
  File "/usr/lib/python2.7/subprocess.py", line 1301, in wait
    time.sleep(1.5)
KeyboardInterrupt
    pid, sts = _eintr_retry_call(os.waitpid, self.pid, 0)
  File "/usr/lib/python2.7/subprocess.py", line 478, in _eintr_retry_call
    return func(*args)
KeyboardInterrupt
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m echo '{"rate": 1.5, "duration": 30, "temp": "absolute"}$
^[[D^[[D^[[D^[[D{
  "temp": "absolute",
  "recieved": true,
  "rate": 1.5,
  "timestamp": "2015-09-24T14:50:47.589851",
  "duration": 30
}^CTraceback (most recent call last):
Traceback (most recent call last):
  File "/usr/local/bin/openaps", line 5, in <module>
    pkg_resources.run_script('openaps==0.0.6', 'openaps')
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 499, in run_script
    self.require(requires)[0].run_script(script_name, ns)
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 1235, in run_script
    execfile(script_filename, namespace, namespace)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps", line 158, in <module>
    app( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 44, in __call__
    self.run(self.args)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps", line 152, in run
    exit(call(['openaps-%s' % args.command ] + args.args))
  File "/usr/lib/python2.7/subprocess.py", line 493, in call
      File "/usr/local/bin/openaps-use", line 5, in <module>
    pkg_resources.run_script('openaps==0.0.6', 'openaps-use')
return Popen(*popenargs, **kwargs).wait()
  File "/usr/lib/python2.7/subprocess.py", line 1301, in wait
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 499, in run_script
    self.require(requires)[0].run_script(script_name, ns)
    pid, sts = _eintr_retry_call(os.waitpid, self.pid, 0)
  File "/usr/lib/python2.7/subprocess.py", line 478, in _eintr_retry_call
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 1235, in run_script
    return func(*args)
KeyboardInterrupt
    execfile(script_filename, namespace, namespace)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-use", line 63, in <module>
    app( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 45, in __call__
    self.epilog( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-use", line 50, in epilog
    super(UseToolApp, self).epilog( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 64, in epilog
    self.create_git_commit( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 71, in create_git_commit
    self.git_repo( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 66, in git_repo
    from git import Repo
  File "/usr/local/lib/python2.7/dist-packages/GitPython-1.0.1-py2.7.egg/git/__init__.py", line 10, in <module>
    import inspect
  File "/usr/lib/python2.7/inspect.py", line 261, in <module>
    Attribute = namedtuple('Attribute', 'name kind defining_class object')
  File "/usr/lib/python2.7/collections.py", line 353, in namedtuple
    for name in field_names),
  File "/usr/lib/python2.7/collections.py", line 353, in <genexpr>
    for name in field_names),
KeyboardInterrupt
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m echo '{"rate": 1.5, "duration": 30, "temp": "absolute"}$
Traceback (most recent call last):
  File "/usr/local/bin/openaps-use", line 5, in <module>
    pkg_resources.run_script('openaps==0.0.6', 'openaps-use')
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 499, in run_script
    self.require(requires)[0].run_script(script_name, ns)
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 1235, in run_script
    execfile(script_filename, namespace, namespace)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-use", line 63, in <module>
    app( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 44, in __call__
    self.run(self.args)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-use", line 57, in run
    output = app(args, self)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/__init__.py", line 92, in __call__
    return self.method.selected(args)(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/__init__.py", line 31, in __call__
    return self.method(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/use.py", line 26, in __call__
    output = self.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/vendors/medtronic.py", line 279, in main
    results = self.upload_program(program)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/vendors/medtronic.py", line 288, in upload_program
    return self.pump.model.set_temp_basal(**program)
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/models/__init__.py", line 182, in set_temp_basal
    result = self._set_temp_basal(**basals)
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/models/__init__.py", line 22, in __call__
    self.response = inst.session.query(self.msg, **kwds)
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/session.py", line 110, in query
    self.execute(command)
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/session.py", line 107, in execute
    return super(type(self), self).execute(command)
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/session.py", line 39, in execute
    self.download( )
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/session.py", line 54, in download
    self.command.respond(data)
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/commands.py", line 55, in respond
    self.getData( )
  File "/usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg/decocare/commands.py", line 248, in getData
    received = True if self.data[0] is 0 else False
IndexError: bytearray index out of range
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m ^M^[[K^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@ras$
pump://JSON/read_settings/read_settings.json
reporting read_settings.json
pump://JSON/read_bg_targets/read_bg_targets.json
reporting read_bg_targets.json
pump://JSON/read_insulin_sensitivies/read_insulin_sensitivies.json
reporting read_insulin_sensitivies.json
pump://JSON/read_selected_basal_profile/read_selected_basal_profile.json
reporting read_selected_basal_profile.json
pump://JSON/read_carb_ratios/read_carb_ratios.json
reporting read_carb_ratios.json
pump://JSON/read_status/read_status.json
reporting read_status.json
pump://JSON/read_battery_status/read_battery_status.json
reporting read_battery_status.json
pump://JSON/read_clock/read_clock.json
reporting read_clock.json
cgm://JSON/iter_glucose_hours/recent_glucose.json
reporting recent_glucose.json
pump://JSON/iter_pump_hours/recent_history.json
reporting recent_history.json
glucose://JSON/clean/clean_glucose.json
reporting clean_glucose.json
munge://JSON/clean/clean_history.json
reporting clean_history.json
munge://JSON/reconcile/reconcile_history.json
reporting reconcile_history.json
munge://JSON/resolve/resolve_history.json
reporting resolve_history.json
munge://JSON/normalize/normalized_history.json
reporting normalized_history.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps predict
predict://JSON/glucose/predict_glucose.json
predict_glucose.json  raised  'int' object has no attribute 'read'
Traceback (most recent call last):
  File "/usr/local/bin/openaps-report", line 5, in <module>
    pkg_resources.run_script('openaps==0.0.6', 'openaps-report')
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 499, in run_script
    self.require(requires)[0].run_script(script_name, ns)
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 1235, in run_script
    execfile(script_filename, namespace, namespace)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-report", line 82, in <module>
    app( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 44, in __call__
    self.run(self.args)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-report", line 75, in run
    output = app(args, self)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/subcommand.py", line 50, in __call__
    return self.method.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/reports/invoke.py", line 40, in main
    output = task.method(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/use.py", line 26, in __call__
    output = self.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg/openapscontrib/predict/__init__.py", line 176, in main
    return future_glucose(*args, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg/openapscontrib/predict/predict.py", line 169, in future_glucose
    last_history_datetime = parse(last_history_event['end_at'])
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 1008, in parse
    return DEFAULTPARSER.parse(timestr, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 392, in parse
    res = self._parse(timestr, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 492, in _parse
    l = _timelex.split(timestr)         # Splits the timestr into tokens
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 174, in split
    return list(cls(s))
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 171, in next
    return self.__next__()  # Python 2.x support
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 164, in __next__
    token = self.get_token()
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 82, in get_token
    nextchar = self.instream.read(1)
AttributeError: 'int' object has no attribute 'read'
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps vendor\^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^H^[$
refresh report invoke read_settings.json read_bg_targets.json read_insulin_sensitivies.json read_selected_basal_profile.json read_carb_ratios.json
update report invoke read_status.json read_battery_status.json read_clock.json recent_glucose.json recent_history.json
munge report invoke clean_glucose.json clean_history.json reconcile_history.json resolve_history.json normalized_history.json
predict report invoke predict_glucose.json predict_glucose_without_future_basal.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps alias show^H^H^H^H^H^H^H^H^H^H^[[3Ppredict
predict://JSON/glucose/predict_glucose.json
predict_glucose.json  raised  'int' object has no attribute 'read'
Traceback (most recent call last):
  File "/usr/local/bin/openaps-report", line 5, in <module>
    pkg_resources.run_script('openaps==0.0.6', 'openaps-report')
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 499, in run_script
    self.require(requires)[0].run_script(script_name, ns)
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 1235, in run_script
    execfile(script_filename, namespace, namespace)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-report", line 82, in <module>
    app( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 44, in __call__
    self.run(self.args)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-report", line 75, in run
    output = app(args, self)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/subcommand.py", line 50, in __call__
    return self.method.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/reports/invoke.py", line 40, in main
    output = task.method(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/use.py", line 26, in __call__
    output = self.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg/openapscontrib/predict/__init__.py", line 176, in main
    return future_glucose(*args, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg/openapscontrib/predict/predict.py", line 169, in future_glucose
    last_history_datetime = parse(last_history_event['end_at'])
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 1008, in parse
    return DEFAULTPARSER.parse(timestr, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 392, in parse
    res = self._parse(timestr, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 492, in _parse
    l = _timelex.split(timestr)         # Splits the timestr into tokens
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 174, in split
    return list(cls(s))
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 171, in next
    return self.__next__()  # Python 2.x support
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 164, in __next__
    token = self.get_token()
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 82, in get_token
    nextchar = self.instream.read(1)
AttributeError: 'int' object has no attribute 'read'
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m predict_glucose_without_future_basal.json^G^G^M^[[C^[[C$
refresh report invoke read_settings.json read_bg_targets.json read_insulin_sensitivies.json read_selected_basal_profile.json read_carb_ratios.json
update report invoke read_status.json read_battery_status.json read_clock.json recent_glucose.json recent_history.json
munge report invoke clean_glucose.json clean_history.json reconcile_history.json resolve_history.json normalized_history.json
predict report invoke predict_glucose.json predict_glucose_without_future_basal.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps report invoke predict_glucose.json JSON ^H^[[K^$
predict://JSON/glucose/predict_glucose.json
predict_glucose.json  raised  'int' object has no attribute 'read'
 Traceback (most recent call last):
  File "/usr/local/bin/openaps-report", line 5, in <module>
    pkg_resources.run_script('openaps==0.0.6', 'openaps-report')
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 499, in run_script
    self.require(requires)[0].run_script(script_name, ns)
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 1235, in run_script
    execfile(script_filename, namespace, namespace)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-report", line 82, in <module>
    app( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 44, in __call__
    self.run(self.args)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-report", line 75, in run
    output = app(args, self)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/subcommand.py", line 50, in __call__
    return self.method.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/reports/invoke.py", line 40, in main
    output = task.method(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/use.py", line 26, in __call__
    output = self.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg/openapscontrib/predict/__init__.py", line 176, in main
    return future_glucose(*args, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg/openapscontrib/predict/predict.py", line 169, in future_glucose
    last_history_datetime = parse(last_history_event['end_at'])
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 1008, in parse
    return DEFAULTPARSER.parse(timestr, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 392, in parse
    res = self._parse(timestr, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 492, in _parse
    l = _timelex.split(timestr)         # Splits the timestr into tokens
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 174, in split
    return list(cls(s))
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 171, in next
    return self.__next__()  # Python 2.x support
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 164, in __next__
    token = self.get_token()
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 82, in get_token
    nextchar = self.instream.read(1)
AttributeError: 'int' object has no attribute 'read'
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m time

real    0m0.000s
user    0m0.000s
sys     0m0.000s
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m date
Thu Sep 24 14:59:49 PDT 2015
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m ls
20150920_1030am          predict_glucose.json                       read_bg_targets.json              read_settings.json      resolve_history.json
clean_glucose.json       predict_glucose_without_future_basal.json  read_carb_ratios.json             read_status.json
clean_history.json       pump-history.json                          read_clock.json                   recent_glucose.json
normalized_history.json  ^[[0m^[[01;34mpump_record_pages^[[0m                          read_insulin_sensitivies.json     recent_history.json
openaps.ini              read_battery_status.json                   read_selected_basal_profile.json  reconcile_history.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m ^M^[[K^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@ras$
added predict://JSON/glucose/predict_glucose.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps report add predict_glucose_without_future_basal$
added predict://JSON/glucose/predict_glucose_without_future_basal.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps report invoke predict_b^H^[[Kglucose_without_fu$
predict://JSON/glucose/predict_glucose_without_future_basal.json
predict_glucose_without_future_basal.json  raised  History data is more than 5 minutes old
Traceback (most recent call last):
  File "/usr/local/bin/openaps-report", line 5, in <module>
    pkg_resources.run_script('openaps==0.0.6', 'openaps-report')
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 499, in run_script
    self.require(requires)[0].run_script(script_name, ns)
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 1235, in run_script
    execfile(script_filename, namespace, namespace)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-report", line 82, in <module>
    app( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 44, in __call__
    self.run(self.args)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-report", line 75, in run
    output = app(args, self)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/subcommand.py", line 50, in __call__
    return self.method.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/reports/invoke.py", line 40, in main
    output = task.method(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/use.py", line 26, in __call__
    output = self.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg/openapscontrib/predict/__init__.py", line 174, in main
    args, kwargs = self.get_program(self.get_params(args))
  File "/usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg/openapscontrib/predict/__init__.py", line 154, in get_program
    assert datetime.now() - pump_history_file_time < timedelta(minutes=5), 'History data is more than 5 minutes old'
AssertionError: History data is more than 5 minutes old
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps report invoke predict_glucose_without_future_ba$
^M^[[K^[[A^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^H^Hdate^H^H^H$
20150920_1030am          predict_glucose.json                       read_bg_targets.json              read_settings.json      resolve_history.json
clean_glucose.json       predict_glucose_without_future_basal.json  read_carb_ratios.json             read_status.json
clean_history.json       pump-history.json                          read_clock.json                   recent_glucose.json
normalized_history.json  ^[[0m^[[01;34mpump_record_pages^[[0m                          read_insulin_sensitivies.json     recent_history.json
openaps.ini              read_battery_status.json                   read_selected_basal_profile.json  reconcile_history.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m ^G ^H^[[Kls^H^Hopenaps report invoke predict_glucose_wi$
predict://JSON/glucose/predict_glucose_without_future_basal.json
predict_glucose_without_future_basal.json  raised  History data is more than 5 minutes old
Traceback (most recent call last):
  File "/usr/local/bin/openaps-report", line 5, in <module>
    pkg_resources.run_script('openaps==0.0.6', 'openaps-report')
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 499, in run_script
    self.require(requires)[0].run_script(script_name, ns)
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 1235, in run_script
    execfile(script_filename, namespace, namespace)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-report", line 82, in <module>
    app( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 44, in __call__
    self.run(self.args)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-report", line 75, in run
    output = app(args, self)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/subcommand.py", line 50, in __call__
    return self.method.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/reports/invoke.py", line 40, in main
    output = task.method(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/use.py", line 26, in __call__
    output = self.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg/openapscontrib/predict/__init__.py", line 174, in main
    args, kwargs = self.get_program(self.get_params(args))
  File "/usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg/openapscontrib/predict/__init__.py", line 154, in get_program
    assert datetime.now() - pump_history_file_time < timedelta(minutes=5), 'History data is more than 5 minutes old'
AssertionError: History data is more than 5 minutes old
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps refresh && ^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K$
pump://JSON/read_status/read_status.json
reporting read_status.json
pump://JSON/read_battery_status/read_battery_status.json
reporting read_battery_status.json
pump://JSON/read_clock/read_clock.json
reporting read_clock.json
cgm://JSON/iter_glucose_hours/recent_glucose.json
reporting recent_glucose.json
pump://JSON/iter_pump_hours/recent_history.json
reporting recent_history.json
glucose://JSON/clean/clean_glucose.json
reporting clean_glucose.json
munge://JSON/clean/clean_history.json
reporting clean_history.json
munge://JSON/reconcile/reconcile_history.json
reporting reconcile_history.json
munge://JSON/resolve/resolve_history.json
reporting resolve_history.json
munge://JSON/normalize/normalized_history.json
reporting normalized_history.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps update && openaps munge^H^H^H^H^H^H^H^H^H^H^H^H$
predict://JSON/glucose/predict_glucose_without_future_basal.json
predict_glucose_without_future_basal.json  raised  'int' object has no attribute 'read'
Traceback (most recent call last):
  File "/usr/local/bin/openaps-report", line 5, in <module>
    pkg_resources.run_script('openaps==0.0.6', 'openaps-report')
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 499, in run_script
    self.require(requires)[0].run_script(script_name, ns)
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 1235, in run_script
    execfile(script_filename, namespace, namespace)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-report", line 82, in <module>
    app( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 44, in __call__
    self.run(self.args)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-report", line 75, in run
    output = app(args, self)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/subcommand.py", line 50, in __call__
    return self.method.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/reports/invoke.py", line 40, in main
    output = task.method(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/use.py", line 26, in __call__
    output = self.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg/openapscontrib/predict/__init__.py", line 176, in main
    return future_glucose(*args, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg/openapscontrib/predict/predict.py", line 169, in future_glucose
    last_history_datetime = parse(last_history_event['end_at'])
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 1008, in parse
    return DEFAULTPARSER.parse(timestr, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 392, in parse
    res = self._parse(timestr, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 492, in _parse
    l = _timelex.split(timestr)         # Splits the timestr into tokens
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 174, in split
    return list(cls(s))
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 171, in next
    return self.__next__()  # Python 2.x support
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 164, in __next__
    token = self.get_token()
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 82, in get_token
    nextchar = self.instream.read(1)
AttributeError: 'int' object has no attribute 'read'
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m ^M^[[K^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@ras$
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m ^C
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps alias show
refresh report invoke read_settings.json read_bg_targets.json read_insulin_sensitivies.json read_selected_basal_profile.json read_carb_ratios.json
update report invoke read_status.json read_battery_status.json read_clock.json recent_glucose.json recent_history.json
munge report invoke clean_glucose.json clean_history.json reconcile_history.json resolve_history.json normalized_history.json
predict report invoke predict_glucose.json predict_glucose_without_future_basal.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps rev^H^[[Kport invoke predict_glucose.json
predict://JSON/glucose/predict_glucose.json
predict_glucose.json  raised  'int' object has no attribute 'read'
Traceback (most recent call last):
  File "/usr/local/bin/openaps-report", line 5, in <module>
    pkg_resources.run_script('openaps==0.0.6', 'openaps-report')
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 499, in run_script
    self.require(requires)[0].run_script(script_name, ns)
  File "/usr/lib/python2.7/dist-packages/pkg_resources.py", line 1235, in run_script
    execfile(script_filename, namespace, namespace)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-report", line 82, in <module>
    app( )
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/__init__.py", line 44, in __call__
    self.run(self.args)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/EGG-INFO/scripts/openaps-report", line 75, in run
    output = app(args, self)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/cli/subcommand.py", line 50, in __call__
    return self.method.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/reports/invoke.py", line 40, in main
    output = task.method(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg/openaps/uses/use.py", line 26, in __call__
    output = self.main(args, app)
  File "/usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg/openapscontrib/predict/__init__.py", line 176, in main
    return future_glucose(*args, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg/openapscontrib/predict/predict.py", line 169, in future_glucose
    last_history_datetime = parse(last_history_event['end_at'])
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 1008, in parse
    return DEFAULTPARSER.parse(timestr, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 392, in parse
    res = self._parse(timestr, **kwargs)
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 492, in _parse
    l = _timelex.split(timestr)         # Splits the timestr into tokens
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 174, in split
    return list(cls(s))
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 171, in next
    return self.__next__()  # Python 2.x support
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 164, in __next__
    token = self.get_token()
  File "/usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg/dateutil/parser.py", line 82, in get_token
    nextchar = self.instream.read(1)
AttributeError: 'int' object has no attribute 'read'
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m ls
20150920_1030am          predict_glucose.json                       read_bg_targets.json              read_settings.json      resolve_history.json
clean_glucose.json       predict_glucose_without_future_basal.json  read_carb_ratios.json             read_status.json
clean_history.json       pump-history.json                          read_clock.json                   recent_glucose.json
normalized_history.json  ^[[0m^[[01;34mpump_record_pages^[[0m                          read_insulin_sensitivies.json     recent_history.json
openaps.ini              read_battery_status.json                   read_selected_basal_profile.json  reconcile_history.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m cd ..^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^Gop^H^[[K^H^[[K^Gca$
[device "pump"]
serial = 524106
vendor = openaps.vendors.medtronic
expires = 2015-09-24T15:15:15.121564
model = 522

[device "cgm"]
vendor = openaps.vendors.dexcom

[report "pump-history.json"]
device = pump
hours = 10.0
use = iter_pump_hours
reporter = JSON

[report "recent_glucose.json"]
device = cgm
hours = 6.0
use = iter_glucose_hours
reporter = JSON

[report "recent_history.json"]
device = pump
hours = 6.0
use = iter_pump_hours
reporter = JSON

[report "read_clock.json"]
device = pump
use = read_clock
reporter = JSON

[report "read_settings.json"]
device = pump
use = read_settings
reporter = JSON

[report "read_selected_basal_profile.json"]
device = pump
use = read_selected_basal_profile
reporter = JSON

[report "read_bg_targets.json"]
device = pump
use = read_bg_targets
reporter = JSON

[report "read_status.json"]
device = pump
use = read_status
reporter = JSON

[report "read_insulin_sensitivies.json"]
device = pump
use = read_insulin_sensitivies
reporter = JSON

[report "read_carb_ratios.json"]
device = pump
use = read_carb_ratios
reporter = JSON

[report "read_battery_status.json"]
device = pump
use = read_battery_status
reporter = JSON

[vendor "openapscontrib.mmhistorytools"]
path = .
module = openapscontrib.mmhistorytools

[device "munge"]
vendor = openapscontrib.mmhistorytools

[vendor "openapscontrib.glucosetools"]
path = .
module = openapscontrib.glucosetools

[device "glucose"]
vendor = openapscontrib.glucosetools

[report "clean_glucose.json"]
device = glucose
use = clean
infile = recent_glucose.json
reporter = JSON

[report "reconcile_history.json"]
device = munge
use = reconcile
infile = clean_history.json
reporter = JSON

[report "resolve_history.json"]
device = munge
use = resolve
infile = reconcile_history.json
reporter = JSON

[report "clean_history.json"]
device = munge
use = clean
infile = recent_history.json
reporter = JSON

[report "normalized_history.json"]
use = normalize
reporter = JSON
basal_profile = read_selected_basal_profile.json
zero_at = read_clock.json
device = munge
infile = resolve_history.json

[alias]
refresh = report invoke read_settings.json read_bg_targets.json read_insulin_sensitivies.json read_selected_basal_profile.json read_carb_ratios.json
update = report invoke read_status.json read_battery_status.json read_clock.json recent_glucose.json recent_history.json
munge = report invoke clean_glucose.json clean_history.json reconcile_history.json resolve_history.json normalized_history.json
predict = report invoke predict_glucose.json predict_glucose_without_future_basal.json

[vendor "openapscontrib.predict"]
path = .
module = openapscontrib.predict

[device "predict"]
vendor = openapscontrib.predict

[report "predict_glucose.json"]
use = glucose
settings = read_settings.json
reporter = JSON
carb_ratios = read_carb_ratios.json
pump-history = normalized_history.json
device = predict
insulin_sensitivities = read_insulin_sensitivies.json
glucose = recent_glucose.json

[report "predict_glucose_without_future_basal.json"]
use = glucose
settings = read_settings.json
reporter = JSON
carb_ratios = read_carb_ratios.json
pump-history = normalized_history.json
device = predict
insulin_sensitivities = read_insulin_sensitivies.json
basal_dosing_end = read_clock.json
glucose = recent_glucose.json

[device "purple"]
serial = 323838
vendor = openaps.vendors.medtronic
expires = 2015-09-24T14:51:51.415920
model = 523

^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m ^C
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m open^H^[[K^H^[[K^H^[[K^H^[[K^Gcat normalizedhost^H^[[K^$
[
  {
    "amount": 0.7999999999999999,
    "start_at": -16,
    "description": "TempBasal: 1.5U/hour over 30min",
    "type": "TempBasal",
    "unit": "U/hour",
    "end_at": 14
  },
  {
    "amount": 0.7999999999999999,
    "start_at": -17,
    "description": "TempBasal: 1.5U/hour over 1min",
    "type": "TempBasal",
    "unit": "U/hour",
    "end_at": -16
  },
  {
    "start_at": -31,
    "description": "Normal bolus: 1.0U",
    "end_at": -31,
    "amount": 1.0,
    "type": "Bolus",
    "unit": "U"
  }
]^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m ^C
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m ^M^[[K^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@ras$
[device "pump"]
serial = 524106
vendor = openaps.vendors.medtronic
expires = 2015-09-24T15:15:15.121564
model = 522

[device "cgm"]
vendor = openaps.vendors.dexcom

[report "pump-history.json"]
device = pump
hours = 10.0
use = iter_pump_hours
reporter = JSON

[report "recent_glucose.json"]
device = cgm
hours = 6.0
use = iter_glucose_hours
reporter = JSON

[report "recent_history.json"]
device = pump
hours = 6.0
use = iter_pump_hours
[report "read_clock.json"]
device = pump
use = read_clock
reporter = JSON

[report "read_settings.json"]
device = pump
use = read_settings
reporter = JSON

[report "read_selected_basal_profile.json"]
device = pump
use = read_selected_basal_profile
reporter = JSON

[report "read_bg_targets.json"]
device = pump
use = read_bg_targets
reporter = JSON

[report "read_status.json"]
device = pump
use = read_status
reporter = JSON

[report "read_insulin_sensitivies.json"]
device = pump
use = read_insulin_sensitivies
reporter = JSON

[report "read_carb_ratios.json"]
device = pump
use = read_carb_ratios
reporter = JSON

[report "read_battery_status.json"]
device = pump
use = read_battery_status
reporter = JSON

[vendor "openapscontrib.mmhistorytools"]
path = .
module = openapscontrib.mmhistorytools

[device "munge"]
vendor = openapscontrib.mmhistorytools

[vendor "openapscontrib.glucosetools"]
path = .
module = openapscontrib.glucosetools

[device "glucose"]
vendor = openapscontrib.glucosetools

[report "clean_glucose.json"]
device = glucose
use = clean
infile = recent_glucose.json
reporter = JSON

[report "reconcile_history.json"]
device = munge
use = reconcile
infile = clean_history.json
reporter = JSON

[report "resolve_history.json"]
device = munge
use = resolve
infile = reconcile_history.json
reporter = JSON

[report "clean_history.json"]
device = munge
use = clean
infile = recent_history.json
reporter = JSON

[report "normalized_history.json"]
use = normalize
reporter = JSON
basal_profile = read_selected_basal_profile.json
zero_at = read_clock.json
device = munge
infile = resolve_history.json

[alias]
refresh = report invoke read_settings.json read_bg_targets.json read_insulin_sensitivies.json read_selected_basal_profile.json read_carb_ratios.json
update = report invoke read_status.json read_battery_status.json read_clock.json recent_glucose.json recent_history.json
munge = report invoke clean_glucose.json clean_history.json reconcile_history.json resolve_history.json normalized_history.json
predict = report invoke predict_glucose.json predict_glucose_without_future_basal.json

[vendor "openapscontrib.predict"]
path = .
module = openapscontrib.predict

[device "predict"]
vendor = openapscontrib.predict

[report "predict_glucose.json"]
use = glucose
settings = read_settings.json
reporter = JSON
carb_ratios = read_carb_ratios.json
pump-history = normalized_history.json
device = predict
insulin_sensitivities = read_insulin_sensitivies.json
glucose = recent_glucose.json

[report "predict_glucose_without_future_basal.json"]
use = glucose
settings = read_settings.json
reporter = JSON
carb_ratios = read_carb_ratios.json
pump-history = normalized_history.json
device = predict
insulin_sensitivities = read_insulin_sensitivies.json
basal_dosing_end = read_clock.json
glucose = recent_glucose.json

[device "purple"]
serial = 323838
vendor = openaps.vendors.medtronic
expires = 2015-09-24T14:51:51.415920
model = 523

^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps report remove normalized_history.json
removed munge://JSON/normalize/normalized_history.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps report add nomraliz^H^[[K^H^[[K^H^[[K^H^[[K^H^[$
^M^[[K^[[A^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[[C^[$
added munge://JSON/normalize/normalized_history.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps refresh^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^H^[$
pump://JSON/read_status/read_status.json
reporting read_status.json
pump://JSON/read_battery_status/read_battery_status.json
reporting read_battery_status.json
pump://JSON/read_clock/read_clock.json
reporting read_clock.json
cgm://JSON/iter_glucose_hours/recent_glucose.json
reporting recent_glucose.json
pump://JSON/iter_pump_hours/recent_history.json
reporting recent_history.json
glucose://JSON/clean/clean_glucose.json
reporting clean_glucose.json
munge://JSON/clean/clean_history.json
reporting clean_history.json
munge://JSON/reconcile/reconcile_history.json
reporting reconcile_history.json
munge://JSON/resolve/resolve_history.json
reporting resolve_history.json
munge://JSON/normalize/normalized_history.json
reporting normalized_history.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m openaps predict
predict://JSON/glucose/predict_glucose.json
reporting predict_glucose.json
predict://JSON/glucose/predict_glucose_without_future_basal.json
reporting predict_glucose_without_future_basal.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m cat predict-^H^[[K_glucose^G
predict_glucose.json                       predict_glucose_without_future_basal.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m cat predict_glucose
predict_glucose.json                       predict_glucose_without_future_basal.json
^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m cat predict_glucose_without_future_basal.json
[
  {
    "date": "2015-09-24T15:16:59",
    "glucose": 125.0
  },
  {
    "date": "2015-09-24T15:21:59",
    "glucose": 123.3117218158675
  },
  {
    "date": "2015-09-24T15:26:59",
    "glucose": 121.43072048207873
  },
  {
    "date": "2015-09-24T15:31:59",
    "glucose": 119.37207646292593
  },
  {
    "date": "2015-09-24T15:36:59",
    "glucose": 117.1545804050257
  },
  {
    "date": "2015-09-24T15:41:59",
    "glucose": 114.81436498345477
  },
  {
    "date": "2015-09-24T15:46:59",
    "glucose": 112.3874701392532
  },
  {
    "date": "2015-09-24T15:51:59",
    "glucose": 109.90690398178107
  },
  {
    "date": "2015-09-24T15:56:59",
    "glucose": 107.40264278871848
  },
  {
    "date": "2015-09-24T16:01:59",
    "glucose": 104.90163100606547
  },
  {
    "date": "2015-09-24T16:06:59",
    "glucose": 102.42778124814217
  },
  {
    "date": "2015-09-24T16:11:59",
    "glucose": 100.00197429758865
  },
  {
    "date": "2015-09-24T16:16:59",
    "glucose": 97.64205910536494
  },
  {
    "date": "2015-09-24T16:21:59",
    "glucose": 95.36285279075118
  },
  {
    "date": "2015-09-24T16:26:59",
    "glucose": 93.17614064134743
  },
  {
    "date": "2015-09-24T16:31:59",
    "glucose": 91.09067611307376
  },
  {
    "date": "2015-09-24T16:36:59",
    "glucose": 89.11218083017025
  },
  {
    "date": "2015-09-24T16:41:59",
    "glucose": 87.24334458519701
  },
  {
    "date": "2015-09-24T16:46:59",
    "glucose": 85.48382533903408
  },
  {
    "date": "2015-09-24T16:51:59",
    "glucose": 83.83024922088157
  },
  {
    "date": "2015-09-24T16:56:59",
    "glucose": 82.27621052825953
  },
  {
    "date": "2015-09-24T17:01:59",
    "glucose": 80.81227172700807
  },
  {
    "date": "2015-09-24T17:06:59",
    "glucose": 79.42596345128726
  },
  {
    "date": "2015-09-24T17:11:59",
    "glucose": 78.10178450357715
  },
  {
    "date": "2015-09-24T17:16:59",
    "glucose": 76.82120185467787
  },
  {
    "date": "2015-09-24T17:21:59",
    "glucose": 75.5626506437095
  },
  {
    "date": "2015-09-24T17:26:59",
    "glucose": 74.30153417811209
  },
  {
    "date": "2015-09-24T17:31:59",
    "glucose": 73.0102239336457
  },
  {
    "date": "2015-09-24T17:36:59",
    "glucose": 71.6580595543904
  },
  {
    "date": "2015-09-24T17:41:59",
    "glucose": 70.2113488527464
  },
  {
    "date": "2015-09-24T17:46:59",
    "glucose": 69.14502455582803
  },
  {
    "date": "2015-09-24T17:51:59",
    "glucose": 68.79408435248124
  },
  {
    "date": "2015-09-24T17:56:59",
    "glucose": 68.4296842061359
  },
  {
    "date": "2015-09-24T18:01:59",
    "glucose": 68.05382007747478
  },
  {
    "date": "2015-09-24T18:06:59",
    "glucose": 67.72489663613757
  },
  {
    "date": "2015-09-24T18:11:59",
    "glucose": 67.45267879980813
  },
  {
    "date": "2015-09-24T18:16:59",
    "glucose": 67.23973136067013
  },
  {
    "date": "2015-09-24T18:21:59",
    "glucose": 67.09111071951682
  },
  {
    "date": "2015-09-24T18:26:59",
    "glucose": 67.01254610373579
  },
  {
    "date": "2015-09-24T18:31:59",
    "glucose": 67.00143573769911
  }
]^[]0;pi@raspberrypi: ~/myopenaps^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/myopenaps $^[[00m cd
^[]0;pi@raspberrypi: ~^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~ $^[[00m ls^H^[[K^H^[[Kgit close git^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^H^[[Kne https://g$
Cloning into 'openaps-monitor'...
remote: Counting objects: 103, done.^[[K
remote: Compressing objects:  33% (1/3)   ^[[K^Mremote: Compressing objects:  66% (2/3)   ^[[K^Mremote: Compressing objects: 100% (3/3)   ^[[K^Mremo$
Receiving objects:   0% (1/103)   ^MReceiving objects:   1% (2/103)   ^MReceiving objects:   2% (3/103)   ^MReceiving objects:   3% (4/103)   ^MRece$
Receiving objects:  45% (47/103)   ^MReceiving objects:  46% (48/103)   ^MReceiving objects:  47% (49/103)   ^MReceiving objects:  48% (50/103)   ^M$
Resolving deltas:   0% (0/50)   ^MResolving deltas:   6% (3/50)   ^MResolving deltas:   8% (4/50)   ^MResolving deltas:  20% (10/50)   ^MResolving d$
^[]0;pi@raspberrypi: ~^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~ $^[[00m c^H^[[K^G^Gcd openaps-monitor
^[]0;pi@raspberrypi: ~/openaps-monitor^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/openaps-monitor $^[[00m pip install -r p^H^[[Krequirements.txt
bash: pip: command not found
^[]0;pi@raspberrypi: ~/openaps-monitor^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/openaps-monitor $^[[00m pip freeze
bash: pip: command not found
^[]0;pi@raspberrypi: ~/openaps-monitor^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/openaps-monitor $^[[00m pip^H^[[K^H^[[K^H^[[Ksudo apt ^H^[[K-get in$
^MReading package lists... 0%^M^MReading package lists... 100%^M^MReading package lists... Done^M
^MBuilding dependency tree... 0%^M^MBuilding dependency tree... 0%^M^MBuilding dependency tree... 1%^M^MBuilding dependency tree... 50%^M^MBuilding $
^MReading state information... 0%^M^MReading state information... 0%^M^MReading state information... Done^M
The following extra packages will be installed:
  python2.6 python2.6-minimal
Suggested packages:
  python2.6-doc binfmt-support
Recommended packages:
  python-dev-all
The following NEW packages will be installed:
  python-pip python2.6 python2.6-minimal
0 upgraded, 3 newly installed, 0 to remove and 0 not upgraded.
Need to get 3,962 kB of archives.
After this operation, 13.2 MB of additional disk space will be used.
Do you want to continue [Y/n]? y
^M^M0% [Working]^M            ^M0% [Connecting to mirrordirector.raspbian.org]^M0% [Connecting to mirrordirector.raspbian.org]^M                    $
^M            ^M0% [1 python2.6-minimal 0 B/1,409 kB 0%] [Waiting for headers]^M                                                              ^M0% [$
^M             ^M36% [2 python2.6 0 B/2,442 kB 0%]^M                                 ^M46% [2 python2.6 398 kB/2,442 kB 16%]^M46% [2 python2.6 419 k$
^M97% [3 python-pip 0 B/112 kB 0%]                                                                                                                  $
Selecting previously unselected package python2.6-minimal.
(Reading database ... ^M(Reading database ... 5%^M(Reading database ... 10%^M(Reading database ... 15%^M(Reading database ... 20%^M(Reading database$
Unpacking python2.6-minimal (from .../python2.6-minimal_2.6.8-1.1_armhf.deb) ...
Selecting previously unselected package python2.6.
Unpacking python2.6 (from .../python2.6_2.6.8-1.1_armhf.deb) ...
Selecting previously unselected package python-pip.
Unpacking python-pip (from .../python-pip_1.1-3_all.deb) ...
Processing triggers for man-db ...
Processing triggers for desktop-file-utils ...
Processing triggers for menu ...
Setting up python2.6-minimal (2.6.8-1.1) ...
Linking and byte-compiling packages for runtime python2.6...
Setting up python2.6 (2.6.8-1.1) ...
Setting up python-pip (1.1-3) ...
Processing triggers for python-support ...
Processing triggers for menu ...
^[]0;pi@raspberrypi: ~/openaps-monitor^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/openaps-monitor $^[[00m pip instal -r requirements.txt
Usage: pip COMMAND [OPTIONS]

pip: error: No command by the name pip instal
  (maybe you meant "pip install -r requirements.txt")
^[]0;pi@raspberrypi: ~/openaps-monitor^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/openaps-monitor $^[[00m pip instal -r requirements.txt^H^H^H^H^H^H^$
Downloading/unpacking flask (from -r requirements.txt (line 1))
  Downloading Flask-0.10.1.tar.gz (544Kb): ^M  Downloading Flask-0.10.1.tar.gz (544Kb):   0%  4.1Kb^M  Downloading Flask-0.10.1.tar.gz (544Kb):   1%$
  Running setup.py egg_info for package flask

    warning: no files found matching '*' under directory 'tests'
    warning: no previously-included files matching '*.pyc' found under directory 'docs'
    warning: no previously-included files matching '*.pyo' found under directory 'docs'
    warning: no previously-included files matching '*.pyc' found under directory 'tests'
    warning: no previously-included files matching '*.pyo' found under directory 'tests'
    warning: no previously-included files matching '*.pyc' found under directory 'examples'
    warning: no previously-included files matching '*.pyo' found under directory 'examples'
    no previously-included directories found matching 'docs/_build'
    no previously-included directories found matching 'docs/_themes/.git'
Requirement already satisfied (use --upgrade to upgrade): openapscontrib.predict in /usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.$
Requirement already satisfied (use --upgrade to upgrade): python-dateutil in /usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg $
Downloading/unpacking Werkzeug>=0.7 (from flask->-r requirements.txt (line 1))
  Downloading Werkzeug-0.10.4.tar.gz (1.1Mb): ^M  Downloading Werkzeug-0.10.4.tar.gz (1.1Mb):   0%  4.1Kb^M  Downloading Werkzeug-0.10.4.tar.gz (1.1$
  Running setup.py egg_info for package Werkzeug

    no previously-included directories found matching 'docs/_build'
    no previously-included directories found matching 'docs/_themes'
    warning: no previously-included files matching '*.py[cdo]' found anywhere in distribution
    warning: no previously-included files matching '__pycache__' found anywhere in distribution
    warning: no previously-included files matching '*.so' found anywhere in distribution
    warning: no previously-included files matching '*.pyd' found anywhere in distribution
Downloading/unpacking Jinja2>=2.4 (from flask->-r requirements.txt (line 1))
  Downloading Jinja2-2.8.tar.gz (357Kb): ^M  Downloading Jinja2-2.8.tar.gz (357Kb):   1%  4.1Kb^M  Downloading Jinja2-2.8.tar.gz (357Kb):   2%  8.2K$
  Running setup.py egg_info for package Jinja2

    warning: no files found matching 'run-tests.py'
    warning: no files found matching '*' under directory 'custom_fixers'
    warning: no files found matching '*' under directory 'jinja2/testsuite/res'
    warning: no previously-included files matching '*' found under directory 'docs/_build'
    warning: no previously-included files matching '*.pyc' found under directory 'jinja2'
    warning: no previously-included files matching '*.pyc' found under directory 'docs'
    warning: no previously-included files matching '*.pyo' found under directory 'jinja2'
    warning: no previously-included files matching '*.pyo' found under directory 'docs'
Downloading/unpacking itsdangerous>=0.21 (from flask->-r requirements.txt (line 1))
  Downloading itsdangerous-0.24.tar.gz (46Kb): ^M  Downloading itsdangerous-0.24.tar.gz (46Kb):   8%  4.1Kb^M  Downloading itsdangerous-0.24.tar.gz $
  Running setup.py egg_info for package itsdangerous

    warning: no previously-included files matching '*' found under directory 'docs/_build'
Requirement already satisfied (use --upgrade to upgrade): openapscontrib.mmhistorytools in /usr/local/lib/python2.7/dist-packages/openapscontrib.mmh$
Requirement already satisfied (use --upgrade to upgrade): six>=1.5 in /usr/local/lib/python2.7/dist-packages/six-1.9.0-py2.7.egg (from python-dateut$
Downloading/unpacking MarkupSafe (from Jinja2>=2.4->flask->-r requirements.txt (line 1))
  Downloading MarkupSafe-0.23.tar.gz
  Running setup.py egg_info for package MarkupSafe

Requirement already satisfied (use --upgrade to upgrade): openaps in /usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg (from openapscon$
Requirement already satisfied (use --upgrade to upgrade): pyserial in /usr/lib/python2.7/dist-packages (from openaps->openapscontrib.mmhistorytools-$
Requirement already satisfied (use --upgrade to upgrade): argcomplete in /usr/local/lib/python2.7/dist-packages/argcomplete-1.0.0-py2.7.egg (from op$
Requirement already satisfied (use --upgrade to upgrade): gitpython in /usr/local/lib/python2.7/dist-packages/GitPython-1.0.1-py2.7.egg (from openap$
Requirement already satisfied (use --upgrade to upgrade): decocare>0.0.16 in /usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg (f$
Requirement already satisfied (use --upgrade to upgrade): dexcom-reader>0.0.5 in /usr/local/lib/python2.7/dist-packages/dexcom_reader-0.0.7-py2.7.eg$
Requirement already satisfied (use --upgrade to upgrade): gitdb>=0.6.4 in /usr/local/lib/python2.7/dist-packages/gitdb-0.6.4-py2.7-linux-armv7l.egg $
Requirement already satisfied (use --upgrade to upgrade): smmap>=0.8.5 in /usr/local/lib/python2.7/dist-packages/smmap-0.9.0-py2.7.egg (from gitdb>=$
Installing collected packages: flask, Werkzeug, Jinja2, itsdangerous, MarkupSafe
  Running setup.py install for flask

    warning: no files found matching '*' under directory 'tests'
    warning: no previously-included files matching '*.pyc' found under directory 'docs'
    warning: no previously-included files matching '*.pyo' found under directory 'docs'
    warning: no previously-included files matching '*.pyc' found under directory 'tests'
    warning: no previously-included files matching '*.pyo' found under directory 'tests'
    warning: no previously-included files matching '*.pyc' found under directory 'examples'
    warning: no previously-included files matching '*.pyo' found under directory 'examples'
    no previously-included directories found matching 'docs/_build'
    no previously-included directories found matching 'docs/_themes/.git'
    error: could not create '/usr/local/lib/python2.7/dist-packages/flask': Permission denied
    Complete output from command /usr/bin/python -c "import setuptools;__file__='/home/pi/openaps-monitor/build/flask/setup.py';exec(compile(open(__$
    running install

running build

running build_py

creating build

creating build/lib.linux-armv7l-2.7

creating build/lib.linux-armv7l-2.7/flask

copying flask/sessions.py -> build/lib.linux-armv7l-2.7/flask

copying flask/json.py -> build/lib.linux-armv7l-2.7/flask

copying flask/debughelpers.py -> build/lib.linux-armv7l-2.7/flask

copying flask/module.py -> build/lib.linux-armv7l-2.7/flask

copying flask/blueprints.py -> build/lib.linux-armv7l-2.7/flask

copying flask/views.py -> build/lib.linux-armv7l-2.7/flask

copying flask/config.py -> build/lib.linux-armv7l-2.7/flask

copying flask/app.py -> build/lib.linux-armv7l-2.7/flask

copying flask/_compat.py -> build/lib.linux-armv7l-2.7/flask

copying flask/wrappers.py -> build/lib.linux-armv7l-2.7/flask

copying flask/templating.py -> build/lib.linux-armv7l-2.7/flask

copying flask/__init__.py -> build/lib.linux-armv7l-2.7/flask

copying flask/globals.py -> build/lib.linux-armv7l-2.7/flask

copying flask/logging.py -> build/lib.linux-armv7l-2.7/flask

copying flask/testing.py -> build/lib.linux-armv7l-2.7/flask

copying flask/exthook.py -> build/lib.linux-armv7l-2.7/flask

copying flask/signals.py -> build/lib.linux-armv7l-2.7/flask

copying flask/helpers.py -> build/lib.linux-armv7l-2.7/flask

copying flask/ctx.py -> build/lib.linux-armv7l-2.7/flask

creating build/lib.linux-armv7l-2.7/flask/ext

copying flask/ext/__init__.py -> build/lib.linux-armv7l-2.7/flask/ext

creating build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/examples.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/blueprints.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/views.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/config.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/appctx.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/regression.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/basic.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/subclassing.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/templating.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/deprecations.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/ext.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/testing.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/signals.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/reqctx.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/helpers.py -> build/lib.linux-armv7l-2.7/flask/testsuite

running egg_info

writing requirements to Flask.egg-info/requires.txt

writing Flask.egg-info/PKG-INFO

writing top-level names to Flask.egg-info/top_level.txt

writing dependency_links to Flask.egg-info/dependency_links.txt

warning: manifest_maker: standard file '-c' not found



reading manifest file 'Flask.egg-info/SOURCES.txt'

reading manifest template 'MANIFEST.in'

warning: no files found matching '*' under directory 'tests'

warning: no previously-included files matching '*.pyc' found under directory 'docs'

warning: no previously-included files matching '*.pyo' found under directory 'docs'

warning: no previously-included files matching '*.pyc' found under directory 'tests'

warning: no previously-included files matching '*.pyo' found under directory 'tests'

warning: no previously-included files matching '*.pyc' found under directory 'examples'

warning: no previously-included files matching '*.pyo' found under directory 'examples'

no previously-included directories found matching 'docs/_build'

no previously-included directories found matching 'docs/_themes/.git'

writing manifest file 'Flask.egg-info/SOURCES.txt'

creating build/lib.linux-armv7l-2.7/flask/testsuite/static

copying flask/testsuite/static/index.html -> build/lib.linux-armv7l-2.7/flask/testsuite/static

creating build/lib.linux-armv7l-2.7/flask/testsuite/templates

copying flask/testsuite/templates/_macro.html -> build/lib.linux-armv7l-2.7/flask/testsuite/templates

copying flask/testsuite/templates/context_template.html -> build/lib.linux-armv7l-2.7/flask/testsuite/templates

copying flask/testsuite/templates/escaping_template.html -> build/lib.linux-armv7l-2.7/flask/testsuite/templates

copying flask/testsuite/templates/mail.txt -> build/lib.linux-armv7l-2.7/flask/testsuite/templates

copying flask/testsuite/templates/simple_template.html -> build/lib.linux-armv7l-2.7/flask/testsuite/templates

copying flask/testsuite/templates/template_filter.html -> build/lib.linux-armv7l-2.7/flask/testsuite/templates

copying flask/testsuite/templates/template_test.html -> build/lib.linux-armv7l-2.7/flask/testsuite/templates

creating build/lib.linux-armv7l-2.7/flask/testsuite/templates/nested

copying flask/testsuite/templates/nested/nested.txt -> build/lib.linux-armv7l-2.7/flask/testsuite/templates/nested

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps

copying flask/testsuite/test_apps/config_module_app.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps

copying flask/testsuite/test_apps/flask_newext_simple.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps

copying flask/testsuite/test_apps/importerror.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps

copying flask/testsuite/test_apps/main_app.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp

copying flask/testsuite/test_apps/blueprintapp/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps

copying flask/testsuite/test_apps/blueprintapp/apps/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/admin

copying flask/testsuite/test_apps/blueprintapp/apps/admin/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/admin

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/admin/static

copying flask/testsuite/test_apps/blueprintapp/apps/admin/static/test.txt -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/admin/static/css

copying flask/testsuite/test_apps/blueprintapp/apps/admin/static/css/test.css -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/a$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/admin/templates

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/admin/templates/admin

copying flask/testsuite/test_apps/blueprintapp/apps/admin/templates/admin/index.html -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/bluepri$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/frontend

copying flask/testsuite/test_apps/blueprintapp/apps/frontend/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/f$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/frontend/templates

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/frontend/templates/frontend

copying flask/testsuite/test_apps/blueprintapp/apps/frontend/templates/frontend/index.html -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/b$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/config_package_app

copying flask/testsuite/test_apps/config_package_app/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/config_package_app

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flask_broken

copying flask/testsuite/test_apps/flask_broken/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flask_broken

copying flask/testsuite/test_apps/flask_broken/b.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flask_broken

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flask_newext_package

copying flask/testsuite/test_apps/flask_newext_package/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flask_newext_package

copying flask/testsuite/test_apps/flask_newext_package/submodule.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flask_newext_package

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flaskext

copying flask/testsuite/test_apps/flaskext/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flaskext

copying flask/testsuite/test_apps/flaskext/oldext_simple.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flaskext

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flaskext/oldext_package

copying flask/testsuite/test_apps/flaskext/oldext_package/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flaskext/oldext_package

copying flask/testsuite/test_apps/flaskext/oldext_package/submodule.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flaskext/oldext_packa$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/lib

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/lib/python2.5

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/lib/python2.5/site-packages

copying flask/testsuite/test_apps/lib/python2.5/site-packages/SiteEgg.egg -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/lib/python2.5/site$

copying flask/testsuite/test_apps/lib/python2.5/site-packages/site_app.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/lib/python2.5/site$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/lib/python2.5/site-packages/site_package

copying flask/testsuite/test_apps/lib/python2.5/site-packages/site_package/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/lib/p$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp

copying flask/testsuite/test_apps/moduleapp/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps

copying flask/testsuite/test_apps/moduleapp/apps/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/admin

copying flask/testsuite/test_apps/moduleapp/apps/admin/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/admin

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/admin/static

copying flask/testsuite/test_apps/moduleapp/apps/admin/static/test.txt -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/admin/$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/admin/static/css

copying flask/testsuite/test_apps/moduleapp/apps/admin/static/css/test.css -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/ad$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/admin/templates

copying flask/testsuite/test_apps/moduleapp/apps/admin/templates/index.html -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/a$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/frontend

copying flask/testsuite/test_apps/moduleapp/apps/frontend/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/frontend

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/frontend/templates

copying flask/testsuite/test_apps/moduleapp/apps/frontend/templates/index.html -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/app$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/path

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/path/installed_package

copying flask/testsuite/test_apps/path/installed_package/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/path/installed_package

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/subdomaintestmodule

copying flask/testsuite/test_apps/subdomaintestmodule/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/subdomaintestmodule

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/subdomaintestmodule/static

copying flask/testsuite/test_apps/subdomaintestmodule/static/hello.txt -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/subdomaintestmodule/s$

running install_lib

creating /usr/local/lib/python2.7/dist-packages/flask

error: could not create '/usr/local/lib/python2.7/dist-packages/flask': Permission denied

----------------------------------------
Command /usr/bin/python -c "import setuptools;__file__='/home/pi/openaps-monitor/build/flask/setup.py';exec(compile(open(__file__).read().replace('\$
Storing complete log in /home/pi/.pip/pip.log
^[]0;pi@raspberrypi: ~/openaps-monitor^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/openaps-monitor $^[[00m p^H^[[Ksudo apt-get install screen
^MReading package lists... 0%^M^MReading package lists... 100%^M^MReading package lists... Done^M
^MBuilding dependency tree... 0%^M^MBuilding dependency tree... 0%^M^MBuilding dependency tree... 50%^M^MBuilding dependency tree... 50%^M^MBuilding$
^MReading state information... 0%^M^MReading state information... 0%^M^MReading state information... Done^M
Suggested packages:
  iselect screenie byobu
The following NEW packages will be installed:
  screen
0 upgraded, 1 newly installed, 0 to remove and 0 not upgraded.
Need to get 650 kB of archives.
After this operation, 850 kB of additional disk space will be used.
^M^M0% [Working]^M            ^M0% [Connecting to mirrordirector.raspbian.org (5.153.225.207)]^M0% [Connecting to mirrordirector.raspbian.org (5.153$
^M                        ^M0% [1 screen 2,395 B/650 kB 0%]^M9% [1 screen 57.0 kB/650 kB 9%]^M                               ^M20% [1 screen 130 kB/$
Selecting previously unselected package screen.
(Reading database ... ^M(Reading database ... 5%^M(Reading database ... 10%^M(Reading database ... 15%^M(Reading database ... 20%^M(Reading database$
Unpacking screen (from .../screen_4.1.0~20120320gitdb59704-7+deb7u1_armhf.deb) ...
Processing triggers for man-db ...
Processing triggers for install-info ...
Setting up screen (4.1.0~20120320gitdb59704-7+deb7u1) ...
^[]0;pi@raspberrypi: ~/openaps-monitor^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/openaps-monitor $^[[00m pip install ^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^$
Traceback (most recent call last):
  File "monitor.py", line 5, in <module>
    from flask import Flask, render_template
ImportError: No module named flask
^[]0;pi@raspberrypi: ~/openaps-monitor^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/openaps-monitor $^[[00m ls^H^[[K^H^[[K c.^H^[[K^H^[[K^H^[[K^Gpip fr$
Warning: cannot find svn location for distribute==0.6.24dev-r0
GitPython==1.0.1
GnuPGInterface==0.3.2
RPi.GPIO==0.5.11
argcomplete==1.0.0
argparse==1.2.1
decocare==0.0.18-dev
dexcom-reader==0.0.7
## FIXME: could not find svn URL in dependency_links for this package:
distribute==0.6.24dev-r0
gitdb==0.6.4
mcpi==0.1.1
numpy==1.6.2
openaps==0.0.6
openapscontrib.glucosetools==0.0.1
openapscontrib.mmhistorytools==0.0.4
openapscontrib.predict==0.0.2
picamera==1.10
pifacecommon==4.1.2
pifacedigitalio==3.0.4
pycurl==7.19.0
pygame==1.9.1release
pygobject==3.8.2
pyserial==2.5
python-apt==0.8.8.2
python-dateutil==2.4.2
six==1.9.0
smmap==0.9.0
unattended-upgrades==0.1
wsgiref==0.1.2
^[]0;pi@raspberrypi: ~/openaps-monitor^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/openaps-monitor $^[[00m sudo apt-get ^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K$
Downloading/unpacking Flask
  Downloading Flask-0.10.1.tar.gz (544Kb): ^M  Downloading Flask-0.10.1.tar.gz (544Kb):   0%  4.1Kb^M  Downloading Flask-0.10.1.tar.gz (544Kb):   1%$
  Running setup.py egg_info for package Flask

    warning: no files found matching '*' under directory 'tests'
    warning: no previously-included files matching '*.pyc' found under directory 'docs'
    warning: no previously-included files matching '*.pyo' found under directory 'docs'
    warning: no previously-included files matching '*.pyc' found under directory 'tests'
    warning: no previously-included files matching '*.pyo' found under directory 'tests'
    warning: no previously-included files matching '*.pyc' found under directory 'examples'
    warning: no previously-included files matching '*.pyo' found under directory 'examples'
    no previously-included directories found matching 'docs/_build'
    no previously-included directories found matching 'docs/_themes/.git'
Downloading/unpacking Werkzeug>=0.7 (from Flask)
  Running setup.py egg_info for package Werkzeug

    no previously-included directories found matching 'docs/_build'
    no previously-included directories found matching 'docs/_themes'
    warning: no previously-included files matching '*.py[cdo]' found anywhere in distribution
    warning: no previously-included files matching '__pycache__' found anywhere in distribution
    warning: no previously-included files matching '*.so' found anywhere in distribution
    warning: no previously-included files matching '*.pyd' found anywhere in distribution
Downloading/unpacking Jinja2>=2.4 (from Flask)
  Running setup.py egg_info for package Jinja2

    warning: no files found matching 'run-tests.py'
    warning: no files found matching '*' under directory 'custom_fixers'
    warning: no files found matching '*' under directory 'jinja2/testsuite/res'
    warning: no previously-included files matching '*' found under directory 'docs/_build'
    warning: no previously-included files matching '*.pyc' found under directory 'jinja2'
    warning: no previously-included files matching '*.pyc' found under directory 'docs'
    warning: no previously-included files matching '*.pyo' found under directory 'jinja2'
    warning: no previously-included files matching '*.pyo' found under directory 'docs'
Downloading/unpacking itsdangerous>=0.21 (from Flask)
  Running setup.py egg_info for package itsdangerous

    warning: no previously-included files matching '*' found under directory 'docs/_build'
Downloading/unpacking MarkupSafe (from Jinja2>=2.4->Flask)
  Running setup.py egg_info for package MarkupSafe

Installing collected packages: Flask, Werkzeug, Jinja2, itsdangerous, MarkupSafe
  Running setup.py install for Flask

    warning: no files found matching '*' under directory 'tests'
    warning: no previously-included files matching '*.pyc' found under directory 'docs'
    warning: no previously-included files matching '*.pyo' found under directory 'docs'
    warning: no previously-included files matching '*.pyc' found under directory 'tests'
    warning: no previously-included files matching '*.pyo' found under directory 'tests'
    warning: no previously-included files matching '*.pyc' found under directory 'examples'
    warning: no previously-included files matching '*.pyo' found under directory 'examples'
    no previously-included directories found matching 'docs/_build'
    no previously-included directories found matching 'docs/_themes/.git'
    error: could not create '/usr/local/lib/python2.7/dist-packages/flask': Permission denied
    Complete output from command /usr/bin/python -c "import setuptools;__file__='/home/pi/openaps-monitor/build/Flask/setup.py';exec(compile(open(__$
    running install

running build

running build_py

creating build

creating build/lib.linux-armv7l-2.7

creating build/lib.linux-armv7l-2.7/flask

copying flask/sessions.py -> build/lib.linux-armv7l-2.7/flask

copying flask/json.py -> build/lib.linux-armv7l-2.7/flask

copying flask/debughelpers.py -> build/lib.linux-armv7l-2.7/flask

copying flask/module.py -> build/lib.linux-armv7l-2.7/flask

copying flask/blueprints.py -> build/lib.linux-armv7l-2.7/flask

copying flask/views.py -> build/lib.linux-armv7l-2.7/flask

copying flask/config.py -> build/lib.linux-armv7l-2.7/flask

copying flask/app.py -> build/lib.linux-armv7l-2.7/flask

copying flask/_compat.py -> build/lib.linux-armv7l-2.7/flask

copying flask/wrappers.py -> build/lib.linux-armv7l-2.7/flask

copying flask/templating.py -> build/lib.linux-armv7l-2.7/flask

copying flask/__init__.py -> build/lib.linux-armv7l-2.7/flask

copying flask/globals.py -> build/lib.linux-armv7l-2.7/flask

copying flask/logging.py -> build/lib.linux-armv7l-2.7/flask

copying flask/testing.py -> build/lib.linux-armv7l-2.7/flask

copying flask/exthook.py -> build/lib.linux-armv7l-2.7/flask

copying flask/signals.py -> build/lib.linux-armv7l-2.7/flask

copying flask/helpers.py -> build/lib.linux-armv7l-2.7/flask

copying flask/ctx.py -> build/lib.linux-armv7l-2.7/flask

creating build/lib.linux-armv7l-2.7/flask/ext

copying flask/ext/__init__.py -> build/lib.linux-armv7l-2.7/flask/ext

creating build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/examples.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/blueprints.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/views.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/config.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/appctx.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/regression.py -> build/lib.linux-armv7l-2.7/flask/testsuite
copying flask/testsuite/basic.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/subclassing.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/templating.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/deprecations.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/ext.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/testing.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/signals.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/reqctx.py -> build/lib.linux-armv7l-2.7/flask/testsuite

copying flask/testsuite/helpers.py -> build/lib.linux-armv7l-2.7/flask/testsuite

running egg_info

writing requirements to Flask.egg-info/requires.txt

writing Flask.egg-info/PKG-INFO

writing top-level names to Flask.egg-info/top_level.txt

writing dependency_links to Flask.egg-info/dependency_links.txt

warning: manifest_maker: standard file '-c' not found



reading manifest file 'Flask.egg-info/SOURCES.txt'

reading manifest template 'MANIFEST.in'

warning: no files found matching '*' under directory 'tests'

warning: no previously-included files matching '*.pyc' found under directory 'docs'

warning: no previously-included files matching '*.pyo' found under directory 'docs'

warning: no previously-included files matching '*.pyc' found under directory 'tests'

warning: no previously-included files matching '*.pyo' found under directory 'tests'

warning: no previously-included files matching '*.pyc' found under directory 'examples'

warning: no previously-included files matching '*.pyo' found under directory 'examples'

no previously-included directories found matching 'docs/_build'

no previously-included directories found matching 'docs/_themes/.git'

writing manifest file 'Flask.egg-info/SOURCES.txt'

creating build/lib.linux-armv7l-2.7/flask/testsuite/static

copying flask/testsuite/static/index.html -> build/lib.linux-armv7l-2.7/flask/testsuite/static

creating build/lib.linux-armv7l-2.7/flask/testsuite/templates

copying flask/testsuite/templates/_macro.html -> build/lib.linux-armv7l-2.7/flask/testsuite/templates

copying flask/testsuite/templates/context_template.html -> build/lib.linux-armv7l-2.7/flask/testsuite/templates

copying flask/testsuite/templates/escaping_template.html -> build/lib.linux-armv7l-2.7/flask/testsuite/templates

copying flask/testsuite/templates/mail.txt -> build/lib.linux-armv7l-2.7/flask/testsuite/templates

copying flask/testsuite/templates/simple_template.html -> build/lib.linux-armv7l-2.7/flask/testsuite/templates

copying flask/testsuite/templates/template_filter.html -> build/lib.linux-armv7l-2.7/flask/testsuite/templates

copying flask/testsuite/templates/template_test.html -> build/lib.linux-armv7l-2.7/flask/testsuite/templates

creating build/lib.linux-armv7l-2.7/flask/testsuite/templates/nested

copying flask/testsuite/templates/nested/nested.txt -> build/lib.linux-armv7l-2.7/flask/testsuite/templates/nested

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps

copying flask/testsuite/test_apps/config_module_app.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps

copying flask/testsuite/test_apps/flask_newext_simple.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps

copying flask/testsuite/test_apps/importerror.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps

copying flask/testsuite/test_apps/main_app.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp

copying flask/testsuite/test_apps/blueprintapp/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps

copying flask/testsuite/test_apps/blueprintapp/apps/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/admin

copying flask/testsuite/test_apps/blueprintapp/apps/admin/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/admin

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/admin/static

copying flask/testsuite/test_apps/blueprintapp/apps/admin/static/test.txt -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/admin/static/css

copying flask/testsuite/test_apps/blueprintapp/apps/admin/static/css/test.css -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/a$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/admin/templates

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/admin/templates/admin

copying flask/testsuite/test_apps/blueprintapp/apps/admin/templates/admin/index.html -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/bluepri$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/frontend

copying flask/testsuite/test_apps/blueprintapp/apps/frontend/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/f$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/frontend/templates

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/blueprintapp/apps/frontend/templates/frontend

copying flask/testsuite/test_apps/blueprintapp/apps/frontend/templates/frontend/index.html -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/b$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/config_package_app

copying flask/testsuite/test_apps/config_package_app/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/config_package_app

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flask_broken

copying flask/testsuite/test_apps/flask_broken/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flask_broken

copying flask/testsuite/test_apps/flask_broken/b.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flask_broken

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flask_newext_package

copying flask/testsuite/test_apps/flask_newext_package/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flask_newext_package

copying flask/testsuite/test_apps/flask_newext_package/submodule.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flask_newext_package

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flaskext

copying flask/testsuite/test_apps/flaskext/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flaskext

copying flask/testsuite/test_apps/flaskext/oldext_simple.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flaskext

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flaskext/oldext_package

copying flask/testsuite/test_apps/flaskext/oldext_package/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flaskext/oldext_package

copying flask/testsuite/test_apps/flaskext/oldext_package/submodule.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/flaskext/oldext_packa$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/lib

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/lib/python2.5

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/lib/python2.5/site-packages

copying flask/testsuite/test_apps/lib/python2.5/site-packages/SiteEgg.egg -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/lib/python2.5/site$

copying flask/testsuite/test_apps/lib/python2.5/site-packages/site_app.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/lib/python2.5/site$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/lib/python2.5/site-packages/site_package

copying flask/testsuite/test_apps/lib/python2.5/site-packages/site_package/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/lib/p$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp

copying flask/testsuite/test_apps/moduleapp/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps

copying flask/testsuite/test_apps/moduleapp/apps/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/admin

copying flask/testsuite/test_apps/moduleapp/apps/admin/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/admin

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/admin/static

copying flask/testsuite/test_apps/moduleapp/apps/admin/static/test.txt -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/admin/$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/admin/static/css

copying flask/testsuite/test_apps/moduleapp/apps/admin/static/css/test.css -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/ad$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/admin/templates

copying flask/testsuite/test_apps/moduleapp/apps/admin/templates/index.html -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/a$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/frontend

copying flask/testsuite/test_apps/moduleapp/apps/frontend/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/frontend

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/apps/frontend/templates

copying flask/testsuite/test_apps/moduleapp/apps/frontend/templates/index.html -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/moduleapp/app$

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/path

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/path/installed_package

copying flask/testsuite/test_apps/path/installed_package/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/path/installed_package

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/subdomaintestmodule

copying flask/testsuite/test_apps/subdomaintestmodule/__init__.py -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/subdomaintestmodule

creating build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/subdomaintestmodule/static

copying flask/testsuite/test_apps/subdomaintestmodule/static/hello.txt -> build/lib.linux-armv7l-2.7/flask/testsuite/test_apps/subdomaintestmodule/s$

running install_lib

creating /usr/local/lib/python2.7/dist-packages/flask

error: could not create '/usr/local/lib/python2.7/dist-packages/flask': Permission denied

----------------------------------------
Command /usr/bin/python -c "import setuptools;__file__='/home/pi/openaps-monitor/build/Flask/setup.py';exec(compile(open(__file__).read().replace('\$
Storing complete log in /home/pi/.pip/pip.log
^[]0;pi@raspberrypi: ~/openaps-monitor^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/openaps-monitor $^[[00m sudoe pi^H^[[K^H^[[K^H^[[K^H^[[K^H^[[Ko pip$
Downloading/unpacking Flask
  Running setup.py egg_info for package Flask

    warning: no files found matching '*' under directory 'tests'
    warning: no previously-included files matching '*.pyc' found under directory 'docs'
    warning: no previously-included files matching '*.pyo' found under directory 'docs'
    warning: no previously-included files matching '*.pyc' found under directory 'tests'
    warning: no previously-included files matching '*.pyo' found under directory 'tests'
    warning: no previously-included files matching '*.pyc' found under directory 'examples'
    warning: no previously-included files matching '*.pyo' found under directory 'examples'
    no previously-included directories found matching 'docs/_build'
    no previously-included directories found matching 'docs/_themes/.git'
Downloading/unpacking Werkzeug>=0.7 (from Flask)
  Running setup.py egg_info for package Werkzeug

    no previously-included directories found matching 'docs/_build'
    no previously-included directories found matching 'docs/_themes'
    warning: no previously-included files matching '*.py[cdo]' found anywhere in distribution
    warning: no previously-included files matching '__pycache__' found anywhere in distribution
    warning: no previously-included files matching '*.so' found anywhere in distribution
    warning: no previously-included files matching '*.pyd' found anywhere in distribution
Downloading/unpacking Jinja2>=2.4 (from Flask)
  Running setup.py egg_info for package Jinja2

    warning: no files found matching 'run-tests.py'
    warning: no files found matching '*' under directory 'custom_fixers'
    warning: no files found matching '*' under directory 'jinja2/testsuite/res'
    warning: no previously-included files matching '*' found under directory 'docs/_build'
    warning: no previously-included files matching '*.pyc' found under directory 'jinja2'
    warning: no previously-included files matching '*.pyc' found under directory 'docs'
    warning: no previously-included files matching '*.pyo' found under directory 'jinja2'
    warning: no previously-included files matching '*.pyo' found under directory 'docs'
Downloading/unpacking itsdangerous>=0.21 (from Flask)
  Running setup.py egg_info for package itsdangerous

    warning: no previously-included files matching '*' found under directory 'docs/_build'
Downloading/unpacking MarkupSafe (from Jinja2>=2.4->Flask)
  Running setup.py egg_info for package MarkupSafe

Installing collected packages: Flask, Werkzeug, Jinja2, itsdangerous, MarkupSafe
  Running setup.py install for Flask

    warning: no files found matching '*' under directory 'tests'
    warning: no previously-included files matching '*.pyc' found under directory 'docs'
    warning: no previously-included files matching '*.pyo' found under directory 'docs'
    warning: no previously-included files matching '*.pyc' found under directory 'tests'
    warning: no previously-included files matching '*.pyo' found under directory 'tests'
    warning: no previously-included files matching '*.pyc' found under directory 'examples'
    warning: no previously-included files matching '*.pyo' found under directory 'examples'
    no previously-included directories found matching 'docs/_build'
    no previously-included directories found matching 'docs/_themes/.git'
  Running setup.py install for Werkzeug


    no previously-included directories found matching 'docs/_build'
    no previously-included directories found matching 'docs/_themes'
    warning: no previously-included files matching '*.py[cdo]' found anywhere in distribution
    warning: no previously-included files matching '__pycache__' found anywhere in distribution
    warning: no previously-included files matching '*.so' found anywhere in distribution
    warning: no previously-included files matching '*.pyd' found anywhere in distribution
  Running setup.py install for Jinja2

    warning: no files found matching 'run-tests.py'
    warning: no files found matching '*' under directory 'custom_fixers'
    warning: no files found matching '*' under directory 'jinja2/testsuite/res'
    warning: no previously-included files matching '*' found under directory 'docs/_build'
    warning: no previously-included files matching '*.pyc' found under directory 'jinja2'
    warning: no previously-included files matching '*.pyc' found under directory 'docs'
    warning: no previously-included files matching '*.pyo' found under directory 'jinja2'
    warning: no previously-included files matching '*.pyo' found under directory 'docs'
  Running setup.py install for itsdangerous

    warning: no previously-included files matching '*' found under directory 'docs/_build'
  Running setup.py install for MarkupSafe

    building 'markupsafe._speedups' extension
    gcc -pthread -fno-strict-aliasing -DNDEBUG -g -fwrapv -O2 -Wall -Wstrict-prototypes -fPIC -I/usr/include/python2.7 -c markupsafe/_speedups.c -o $
    gcc -pthread -shared -Wl,-O1 -Wl,-Bsymbolic-functions -Wl,-z,relro build/temp.linux-armv7l-2.7/markupsafe/_speedups.o -o build/lib.linux-armv7l-$
Successfully installed Flask Werkzeug Jinja2 itsdangerous MarkupSafe
Cleaning up...
^[]0;pi@raspberrypi: ~/openaps-monitor^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/openaps-monitor $^[[00m sudo pip install Flask^H^H^H^H^H^H^H^H^H^H^$
static/jquery.js not found, downloading from https://code.jquery.com/jquery-2.1.4.min.js
static/bootstrap.js not found, downloading from https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/js/bootstrap.min.js
static/jsapi.js not found, downloading from https://www.google.com/jsapi
static/chart.js not found, downloading from https://www.google.com/uds/api/visualization/1.1/9543863e4f7c29aa0bc62c0051a89a8a/dygraph,webfontloader,$
static/bootstrap.css not found, downloading from https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap.min.css
static/tooltip.css not found, downloading from https://ajax.googleapis.com/ajax/static/modules/gviz/1.0/core/tooltip.css
static/Roboto.ttf not found, downloading from http://fonts.gstatic.com/s/roboto2/v5/Nd9v8a6GbXQiNddD22JCiwLUuEpTyoUstqEm5AMlJo4.ttf
 * Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
 * Restarting with stat
192.168.43.237 - - [24/Sep/2015 15:57:03] "GET / HTTP/1.1" 200 -
192.168.43.237 - - [24/Sep/2015 15:57:04] "GET /static/bootstrap.css HTTP/1.1" 200 -
192.168.43.237 - - [24/Sep/2015 15:57:04] "GET /static/tooltip.css HTTP/1.1" 200 -
192.168.43.237 - - [24/Sep/2015 15:57:04] "GET /static/styles.css HTTP/1.1" 200 -
192.168.43.237 - - [24/Sep/2015 15:57:04] "GET /static/jquery.js HTTP/1.1" 200 -
192.168.43.237 - - [24/Sep/2015 15:57:04] "GET /static/bootstrap.js HTTP/1.1" 200 -
192.168.43.237 - - [24/Sep/2015 15:57:04] "GET /static/jsapi.js HTTP/1.1" 200 -
192.168.43.237 - - [24/Sep/2015 15:57:04] "GET /static/chart.js HTTP/1.1" 200 -
192.168.43.237 - - [24/Sep/2015 15:57:04] "GET /static/monitor.js HTTP/1.1" 200 -
192.168.43.237 - - [24/Sep/2015 15:57:05] "GET /static/Roboto.ttf HTTP/1.1" 200 -
192.168.43.237 - - [24/Sep/2015 15:57:05] "GET /favicon.ico HTTP/1.1" 404 -
192.168.43.237 - - [24/Sep/2015 16:00:03] "GET / HTTP/1.1" 200 -
192.168.43.237 - - [24/Sep/2015 16:00:04] "GET /static/bootstrap.css HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:00:04] "GET /static/tooltip.css HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:00:04] "GET /static/styles.css HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:00:04] "GET /static/jquery.js HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:00:04] "GET /static/bootstrap.js HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:00:04] "GET /static/jsapi.js HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:00:04] "GET /static/chart.js HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:00:04] "GET /static/monitor.js HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:00:04] "GET /static/Roboto.ttf HTTP/1.1" 304 -
^C^[]0;pi@raspberrypi: ~/openaps-monitor^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/openaps-monitor $^[[00m suod^H^[[K^H^[[Kdo ^H^[[K^H^[[K^H^[[K^H^[$
chart.py  chart.pyc  LICENSE  monitor.py  openaps_reports.py  openaps_reports.pyc  README.md  requirements.txt  ^[[0m^[[01;34mstatic^[[0m  ^[[01;34m$
^[]0;pi@raspberrypi: ~/openaps-monitor^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/openaps-monitor $^[[00m sudo n^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^$
^[[?1049h^[[1;24r^[(B^[[m^[[4l^[[?7h^[[?12l^[[?25h^[[?1h^[=^[[?1h^[=^[[?1h^[=^[[39;49m^[[39;49m^[(B^[[m^[[H^[[2J^[(B^[[0;7m  GNU nano 2.2.6         $
^[[?1049h^[[1;24r^[(B^[[m^[[4l^[[?7h^[[?12l^[[?25h^[[?1h^[=^[[?1h^[=^[[?1h^[=^[[39;49m^[[39;49m^[(B^[[m^[[H^[[2J^[(B^[[0;7m  GNU nano 2.2.6         $
 * Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
 * Restarting with stat
192.168.43.237 - - [24/Sep/2015 16:03:21] "GET / HTTP/1.1" 200 -
192.168.43.237 - - [24/Sep/2015 16:03:22] "GET /static/bootstrap.css HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:03:22] "GET /static/tooltip.css HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:03:22] "GET /static/styles.css HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:03:22] "GET /static/jquery.js HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:03:22] "GET /static/bootstrap.js HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:03:22] "GET /static/jsapi.js HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:03:22] "GET /static/chart.js HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:03:23] "GET /static/monitor.js HTTP/1.1" 304 -
192.168.43.237 - - [24/Sep/2015 16:03:23] "GET /static/Roboto.ttf HTTP/1.1" 304 -
^C^[]0;pi@raspberrypi: ~/openaps-monitor^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/openaps-monitor $^[[00m cd
^[]0;pi@raspberrypi: ~^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~ $^[[00m ls
20150920_254pm  20150920_805pm  20150920_952pm  20150923_213pm_real  20150923_311pm  20150924_159pm  ^[[0m^[[01;34mmyopenaps^[[0m  openaps.ini  ^[[0$
^[]0;pi@raspberrypi: ~^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~ $^[[00m mdk^H^[[K^H^[[Kkdr^H^[[Kir bin
^[]0;pi@raspberrypi: ~^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~ $^[[00m cd bin
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m nan^H^[[K^H^[[K^H^[[K^Gsudo nano start-web.sh
^[[?1049h^[[1;44r^[(B^[[m^[[4l^[[?7h^[[?12l^[[?25h^[[?1h^[=^[[?1h^[=^[[?1h^[=^[[39;49m^[[39;49m^[(B^[[m^[[H^[[2J^[(B^[[0;7m  GNU nano 2.2.6         $
^[[?1049h^[[1;44r^[(B^[[m^[[4l^[[?7h^[[?12l^[[?25h^[[?1h^[=^[[?1h^[=^[[?1h^[=^[[39;49m^[[39;49m^[(B^[[m^[[H^[[2J^[(B^[[0;7m  GNU nano 2.2.6         $
fix-stick.sh  start-web.sh
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m chmod a+xr ./*
chmod: changing permissions of `./fix-stick.sh': Operation not permitted
chmod: changing permissions of `./start-web.sh': Operation not permitted
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m chmod a+xr ./*^H^H^H^H^H^H^H^H^H^H^H^H^H^H^[[1@s^[[1@u^[[1@d^[[1@o^$
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m ls
^[[0m^[[01;32mfix-stick.sh^[[0m  ^[[01;32mstart-web.sh^[[0m
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m sudeo n^H^[[K^H^[[K^H^[[K^H^[[K^H^[[Kdo nano every-five.sh
^[[?1049h^[[1;24r^[(B^[[m^[[4l^[[?7h^[[?12l^[[?25h^[[?1h^[=^[[?1h^[=^[[?1h^[=^[[39;49m^[[39;49m^[(B^[[m^[[H^[[2J^[(B^[[0;7m  GNU nano 2.2.6         $
^[[1;24r^[[8;21H^[[32m||^[[39m^[(B^[[m ^[[32m(^[[39m^[(B^[[mpython -m decocare.stick ^[[32m$(^[[39m^[(B^[[mpython -m decocare.scan^[[32m)^[[39m^[(B^$
every-five.sh  ^[[0m^[[01;32mfix-stick.sh^[[0m  ^[[01;32mstart-web.sh^[[0m
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m ls^H^Hsudo nano every-five.sh^H^H^H^H^H^H^H^H^H^H^H^H^H^H^H^H^H^H^H$
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m ls
^[[0m^[[01;32mevery-five.sh^[[0m  ^[[01;32mfix-stick.sh^[[0m  ^[[01;32mstart-web.sh^[[0m
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m crontab-e^H^H^H^H^H tab-e^H^H^H^H^H^H^[[1Ptab-e^H^H^H^H^H^[[C^[[C^[$
no crontab for pi - using an empty one
^[[?1049h^[[1;24r^[(B^[[m^[[4l^[[?7h^[[?12l^[[?25h^[[?1h^[=^[[?1h^[=^[[?1h^[=^[[39;49m^[[39;49m^[(B^[[m^[[H^[[2J^[(B^[[0;7m  GNU nano 2.2.6         $
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m skud^H^[[K^H^[[K^H^[[Kudo every-^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K^H^[[$
sh: 0: Can't open every-five
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m sudo every-five.sh
sudo: every-five.sh: command not found
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m every-fiveevery^H^[[K^H^[[K^H^[[K^H^[[K^H^[[K.sh
bash: every-five.sh: command not found
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m source every-five.sh
pump://JSON/read_status/read_status.json
reporting read_status.json
pump://JSON/read_battery_status/read_battery_status.json
reporting read_battery_status.json
pump://JSON/read_clock/read_clock.json
reporting read_clock.json
cgm://JSON/iter_glucose_hours/recent_glucose.json
reporting recent_glucose.json
pump://JSON/iter_pump_hours/recent_history.json
reporting recent_history.json
glucose://JSON/clean/clean_glucose.json
reporting clean_glucose.json
munge://JSON/clean/clean_history.json
reporting clean_history.json
munge://JSON/reconcile/reconcile_history.json
reporting reconcile_history.json
munge://JSON/resolve/resolve_history.json
reporting resolve_history.json
munge://JSON/normalize/normalized_history.json
reporting normalized_history.json
predict://JSON/glucose/predict_glucose.json
reporting predict_glucose.json
predict://JSON/glucose/predict_glucose_without_future_basal.json
reporting predict_glucose_without_future_basal.json
/home/pi/bin
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m ^M^[[K^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[$
Power-cycling USB to fix dead Carelink stick
bash: /sys/devices/platform/bcm2708_usb/buspower: No such file or directory
bash: /sys/devices/platform/bcm2708_usb/buspower: No such file or directory
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m source start-web.sh
/home/pi/bin
pump://JSON/read_settings/read_settings.json
reporting read_settings.json
pump://JSON/read_bg_targets/read_bg_targets.json
reporting read_bg_targets.json
pump://JSON/read_insulin_sensitivies/read_insulin_sensitivies.json
reporting read_insulin_sensitivies.json
pump://JSON/read_selected_basal_profile/read_selected_basal_profile.json
reporting read_selected_basal_profile.json
pump://JSON/read_carb_ratios/read_carb_ratios.json
reporting read_carb_ratios.json
/home/pi/bin
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m source start-web.sh^H^H^H^H^H^H^H^H^H^H^H^Hfix-stick.sh
Power-cycling USB to fix dead Carelink stick
bash: /sys/devices/platform/bcm2708_usb/buspower: No such file or directory
bash: /sys/devices/platform/bcm2708_usb/buspower: No such file or directory
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m crontab -e
^[[?1049h^[[1;37r^[(B^[[m^[[4l^[[?7h^[[?12l^[[?25h^[[?1h^[=^[[?1h^[=^[[?1h^[=^[[39;49m^[[39;49m^[(B^[[m^[[H^[[2J^[(B^[[0;7m  GNU nano 2.2.6         $
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m sh firx-^H^[[K^H^[[K^H^[[Kx-stick
sh: 0: Can't open fix-stick
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m sh fix-stick^H^H^H^H^H^H^H^H^H^H^H^H^[[2Pcrontab -e^H^H^H^H^H^H^H^H$
Power-cycling USB to fix dead Carelink stick
bash: /sys/devices/platform/bcm2708_usb/buspower: No such file or directory
bash: /sys/devices/platform/bcm2708_usb/buspower: No such file or directory
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m source every-five.sh
pump://JSON/read_status/read_status.json
reporting read_status.json
pump://JSON/read_battery_status/read_battery_status.json
reporting read_battery_status.json
pump://JSON/read_clock/read_clock.json
reporting read_clock.json
cgm://JSON/iter_glucose_hours/recent_glucose.json
reporting recent_glucose.json
pump://JSON/iter_pump_hours/recent_history.json
reporting recent_history.json
glucose://JSON/clean/clean_glucose.json
reporting clean_glucose.json
munge://JSON/clean/clean_history.json
reporting clean_history.json
munge://JSON/reconcile/reconcile_history.json
reporting reconcile_history.json
munge://JSON/resolve/resolve_history.json
reporting resolve_history.json
munge://JSON/normalize/normalized_history.json
reporting normalized_history.json
predict://JSON/glucose/predict_glucose.json
reporting predict_glucose.json
predict://JSON/glucose/predict_glucose_without_future_basal.json
reporting predict_glucose_without_future_basal.json
/home/pi/bin
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m . ./ ^H^[[Kevery-five
bash: ./every-five: No such file or directory
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m . ./every-five.sh
pump://JSON/read_status/read_status.json
reporting read_status.json
pump://JSON/read_battery_status/read_battery_status.json
reporting read_battery_status.json
pump://JSON/read_clock/read_clock.json
reporting read_clock.json
cgm://JSON/iter_glucose_hours/recent_glucose.json
reporting recent_glucose.json
pump://JSON/iter_pump_hours/recent_history.json
reporting recent_history.json
glucose://JSON/clean/clean_glucose.json
reporting clean_glucose.json
munge://JSON/clean/clean_history.json
reporting clean_history.json
munge://JSON/reconcile/reconcile_history.json
reporting reconcile_history.json
munge://JSON/resolve/resolve_history.json
reporting resolve_history.json
munge://JSON/normalize/normalized_history.json
reporting normalized_history.json
predict://JSON/glucose/predict_glucose.json
reporting predict_glucose.json
predict://JSON/glucose/predict_glucose_without_future_basal.json
reporting predict_glucose_without_future_basal.json
/home/pi/bin
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m . ./every-five.sh^H^H^H^[[K^H^H^H^H^H^H^H^H^H^H^H^H^H^Hsource every$
Power-cycling USB to fix dead Carelink stick
bash: /sys/devices/platform/bcm2708_usb/buspower: No such file or directory
bash: /sys/devices/platform/bcm2708_usb/buspower: No such file or directory
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m . ./fix-stick.sh
Power-cycling USB to fix dead Carelink stick
bash: /sys/devices/platform/bcm2708_usb/buspower: No such file or directory
bash: /sys/devices/platform/bcm2708_usb/buspower: No such file or directory
^[]0;pi@raspberrypi: ~/bin^G^[[01;32mpi@raspberrypi^[[00m ^[[01;34m~/bin $^[[00m . ./fix-stick.sh^H^H^H^H^H^H^H^H^H^H^H^H^H^H^H^Hsource fix-stick.sh$
/dev/ttyUSB0:         4884

Script done on Thu 24 Sep 2015 17:05:39 PDT









```






Th 24 Sep 2015 17:36:47

```
pi@cgmcloud1 ~ $ cat 20150924_536pm
Script started on Thu 24 Sep 2015 17:36:47 PDT
pi@raspberrypi ~ $ cd bin/
pi@raspberrypi ~/bin $ ls
every-five.sh  fix-stick.sh  mylog.log  start-web.sh
pi@raspberrypi ~/bin $ sudo nano mylog.log
pi@raspberrypi ~/bin $ sudo nano mylog.log
pi@raspberrypi ~/bin $ ls
every-five.sh  fix-stick.sh  mylog.log  start-web.sh
pi@raspberrypi ~/bin $ cd ..
pi@raspberrypi ~ $ cd ..
pi@raspberrypi /home $ cd ..
pi@raspberrypi / $ ls
bin  boot  boot.bak  dev  etc  home  lib  lost+found  media  mnt  opt  proc  roo                                                                                      t  run  sbin  selinux  srv  sys  tmp  usr  var
pi@raspberrypi / $ cd etc/
pi@raspberrypi /etc $ ls
adduser.conf            deluser.conf         group             issue.net.orig  m                                                                                      enu             plymouth       resolvconf.conf            terminfo
alternatives            dhcp                 group-            issue.orig      m                                                                                      enu-methods     pm             rmt                        timezone
apm                     dhcp3                gshadow           kbd             m                                                                                      ime.types       polkit-1       rpc                        timidity
apparmor.d              dhcpcd.conf          gshadow-          kernel          m                                                                                      ke2fs.conf      ppp            rpi-issue                  triggerhappy
apt                     dhcpcd.duid          gssapi_mech.conf  ldap            m                                                                                      odprobe.d       profile        rsyslog.conf               ts.conf
avahi                   dictionaries-common  gtk-2.0           ld.so.cache     m                                                                                      odules          profile.d      rsyslog.d                  ucf.conf
bash.bashrc             dillo                gtk-3.0           ld.so.conf      m                                                                                      otd             protocols      samba                      udev
bash_completion         dphys-swapfile       host.conf         ld.so.conf.d    m                                                                                      otd.tail        pulse          screenrc                   ufw
bash_completion.d       dpkg                 hostname          ld.so.preload   m                                                                                      tab             python         securetty                  vim
bindresvport.blacklist  drirc                hosts             libaudit.conf   n                                                                                      anorc           python2.6      security                   watchdog.conf
ca-certificates         emacs                hosts.allow       libnl-3         n                                                                                      etconfig        python2.7      selinux                    weston
ca-certificates.conf    environment          hosts.deny        libpaper.d      n                                                                                      etwork          python3        services                   wgetrc
calendar                esound               idmapd.conf       lightdm         n                                                                                      etworks         python3.2      sgml                       wildmidi
ConsoleKit              fake-hwclock.data    ifplugd           locale.alias    n                                                                                      sswitch.conf    rc0.d          shadow                     wpa_supplicant
console-setup           fb.modes             init              locale.gen      n                                                                                      tp.conf         rc1.d          shadow-                    X11
cron.d                  fonts                init.d            localtime       o                                                                                      penal           rc2.d          shells                     xdg
cron.daily              fstab                initramfs-tools   logcheck        o                                                                                      pt              rc3.d          skel                       xml
cron.hourly             fstab.d              inittab           login.defs      o                                                                                      s-release       rc4.d          ssh                        xpdf
cron.monthly            fuse.conf            inputrc           logrotate.conf  o                                                                                      s-release.orig  rc5.d          ssl
crontab                 gai.conf             insserv           logrotate.d     p                                                                                      am.conf         rc6.d          staff-group-for-usr-local
cron.weekly             gconf                insserv.conf      magic           p                                                                                      am.d            rc.local       sudoers
dbus-1                  gdb                  insserv.conf.d    magic.mime      p                                                                                      apersize        rcS.d          sudoers.d
debconf.conf            ghostscript          iproute2          mailcap         p                                                                                      asswd           request-key.d  sysctl.conf
debian_version          gnome                issue             mailcap.order   p                                                                                      asswd-          resolvconf     sysctl.d
default                 groff                issue.net         manpath.config  p                                                                                      erl             resolv.conf    systemd
pi@raspberrypi /etc $ sudo nano modules
pi@raspberrypi ~/bin $ sudo nano mylog.log
pi@raspberrypi ~/bin $ ls
every-five.sh  fix-stick.sh  mylog.log  start-web.sh
pi@raspberrypi ~/bin $ cd ..
pi@raspberrypi ~ $ cd ..
pi@raspberrypi /home $ cd ..
pi@raspberrypi / $ ls
bin  boot  boot.bak  dev  etc  home  lib  lost+found  media  mnt  opt  proc  root  run  sbin  selinux  srv  sys  tmp  usr  var
pi@raspberrypi / $ cd etc/
pi@raspberrypi /etc $ ls
adduser.conf            deluser.conf         group             issue.net.orig  menu             plymouth       resolvconf.conf            terminfo
alternatives            dhcp                 group-            issue.orig      menu-methods     pm             rmt                        timezone
apm                     dhcp3                gshadow           kbd             mime.types       polkit-1       rpc                        timidity
apparmor.d              dhcpcd.conf          gshadow-          kernel          mke2fs.conf      ppp            rpi-issue                  triggerhappy
apt                     dhcpcd.duid          gssapi_mech.conf  ldap            modprobe.d       profile        rsyslog.conf               ts.conf
avahi                   dictionaries-common  gtk-2.0           ld.so.cache     modules          profile.d      rsyslog.d                  ucf.conf
bash.bashrc             dillo                gtk-3.0           ld.so.conf      motd             protocols      samba                      udev
bash_completion         dphys-swapfile       host.conf         ld.so.conf.d    motd.tail        pulse          screenrc                   ufw
bash_completion.d       dpkg                 hostname          ld.so.preload   mtab             python         securetty                  vim
bindresvport.blacklist  drirc                hosts             libaudit.conf   nanorc           python2.6      security                   watchdog.conf
ca-certificates         emacs                hosts.allow       libnl-3         netconfig        python2.7      selinux                    weston
ca-certificates.conf    environment          hosts.deny        libpaper.d      network          python3        services                   wgetrc
calendar                esound               idmapd.conf       lightdm         networks         python3.2      sgml                       wildmidi
ConsoleKit              fake-hwclock.data    ifplugd           locale.alias    nsswitch.conf    rc0.d          shadow                     wpa_supplicant
console-setup           fb.modes             init              locale.gen      ntp.conf         rc1.d          shadow-                    X11
cron.d                  fonts                init.d            localtime       openal           rc2.d          shells                     xdg
cron.daily              fstab                initramfs-tools   logcheck        opt              rc3.d          skel                       xml
cron.hourly             fstab.d              inittab           login.defs      os-release       rc4.d          ssh                        xpdf
cron.monthly            fuse.conf            inputrc           logrotate.conf  os-release.orig  rc5.d          ssl
crontab                 gai.conf             insserv           logrotate.d     pam.conf         rc6.d          staff-group-for-usr-local
cron.weekly             gconf                insserv.conf      magic           pam.d            rc.local       sudoers
dbus-1                  gdb                  insserv.conf.d    magic.mime      papersize        rcS.d          sudoers.d
debconf.conf            ghostscript          iproute2          mailcap         passwd           request-key.d  sysctl.conf
debian_version          gnome                issue             mailcap.order   passwd-          resolvconf     sysctl.d
default                 groff                issue.net         manpath.config  perl             resolv.conf    systemd
pi@raspberrypi /etc $ sudo nano modules
  GNU nano 2.2.6                                           File: modules

# /etc/modules: kernel modules to load at boot time.
#
# This file contains the names of kernel modules that should be loaded
# at boot time, one per line. Lines beginning with "#" are ignored.
# Parameters can be specified after the module name.

snd-bcm2835

# hardware watchdog
bcm2708_wdog
```



Th 24 Sep 2015 18:11:30

```
pi@cgmcloud1 ~ $ cat 20150924_611pm
Script started on Thu 24 Sep 2015 18:11:30 PDT
pi@raspberrypi ~ $ get clone https://eszcloud@bitbucket.org/channemann/openaps-dose.git
bash: get: command not found
pi@raspberrypi ~ $ git clone https://eszcloud@bitbucket.org/channemann/openaps-dCloning into 'openaps-dose'...
Password for 'https://eszcloud@bitbucket.org':
remote: Counting objects: 126, done.
remote: Compressing objects: 100% (124/124), done.
remote: Total 126 (delta 44), reused 0 (delta 0)
Receiving objects: 100% (126/126), 19.37 KiB, done.
Resolving deltas: 100% (44/44), done.
pi@raspberrypi ~ $ cd openaps-dose/
pi@raspberrypi ~/openaps-dose $ ls
LICENSE  openapscontrib  README.md  setup.py  tests
pi@raspberrypi ~/openaps-dose $ sudo python setup.py develop
running develop
Checking .pth file support in /usr/local/lib/python2.7/dist-packages/
/usr/bin/python -E -c pass
TEST PASSED: /usr/local/lib/python2.7/dist-packages/ appears to support .pth files
running egg_info
creating openapscontrib.dose.egg-info
writing requirements to openapscontrib.dose.egg-info/requires.txt
writing openapscontrib.dose.egg-info/PKG-INFO
writing namespace_packages to openapscontrib.dose.egg-info/namespace_packages.txt
writing top-level names to openapscontrib.dose.egg-info/top_level.txt
writing dependency_links to openapscontrib.dose.egg-info/dependency_links.txt
writing manifest file 'openapscontrib.dose.egg-info/SOURCES.txt'
reading manifest file 'openapscontrib.dose.egg-info/SOURCES.txt'
writing manifest file 'openapscontrib.dose.egg-info/SOURCES.txt'
running build_ext
Creating /usr/local/lib/python2.7/dist-packages/openapscontrib.dose.egg-link (link to .)
Adding openapscontrib.dose 0.0.0 to easy-install.pth file

Installed /home/pi/openaps-dose
Processing dependencies for openapscontrib.dose==0.0.0
Searching for python-dateutil==2.4.2
Best match: python-dateutil 2.4.2
Processing python_dateutil-2.4.2-py2.7.egg
python-dateutil 2.4.2 is already the active version in easy-install.pth

Using /usr/local/lib/python2.7/dist-packages/python_dateutil-2.4.2-py2.7.egg
Searching for openapscontrib.predict==0.0.2
Best match: openapscontrib.predict 0.0.2
Processing openapscontrib.predict-0.0.2-py2.7.egg
openapscontrib.predict 0.0.2 is already the active version in easy-install.pth

Using /usr/local/lib/python2.7/dist-packages/openapscontrib.predict-0.0.2-py2.7.egg
Searching for six==1.9.0
Best match: six 1.9.0
Processing six-1.9.0-py2.7.egg
six 1.9.0 is already the active version in easy-install.pth

Using /usr/local/lib/python2.7/dist-packages/six-1.9.0-py2.7.egg
Searching for openapscontrib.mmhistorytools==0.0.4
Best match: openapscontrib.mmhistorytools 0.0.4
Processing openapscontrib.mmhistorytools-0.0.4-py2.7.egg
openapscontrib.mmhistorytools 0.0.4 is already the active version in easy-install.pth

Using /usr/local/lib/python2.7/dist-packages/openapscontrib.mmhistorytools-0.0.4-py2.7.egg
Searching for openaps==0.0.6
Best match: openaps 0.0.6
Processing openaps-0.0.6-py2.7.egg
openaps 0.0.6 is already the active version in easy-install.pth
Installing openaps-install-udev-rules script to /usr/local/bin
Installing openaps-report script to /usr/local/bin
Installing openaps script to /usr/local/bin
Installing openaps-get script to /usr/local/bin
Installing openaps-vendor script to /usr/local/bin
Installing openaps-suggest script to /usr/local/bin
Installing openaps-use script to /usr/local/bin
Installing openaps-alias script to /usr/local/bin
Installing openaps-enact script to /usr/local/bin
Installing openaps-device script to /usr/local/bin
Installing git-openaps-init script to /usr/local/bin

Using /usr/local/lib/python2.7/dist-packages/openaps-0.0.6-py2.7.egg
Searching for dexcom-reader==0.0.7
Best match: dexcom-reader 0.0.7
Processing dexcom_reader-0.0.7-py2.7.egg
dexcom-reader 0.0.7 is already the active version in easy-install.pth

Using /usr/local/lib/python2.7/dist-packages/dexcom_reader-0.0.7-py2.7.egg
Searching for decocare==0.0.18-dev
Best match: decocare 0.0.18-dev
Processing decocare-0.0.18_dev-py2.7.egg
decocare 0.0.18-dev is already the active version in easy-install.pth
Installing mm-temp-basals.py script to /usr/local/bin
Installing mm-press-key.py script to /usr/local/bin
Installing mm-pretty-csv script to /usr/local/bin
Installing mm-latest.py script to /usr/local/bin
Installing mm-send-comm.py script to /usr/local/bin
Installing mm-decode-history-page.py script to /usr/local/bin
Installing mm-set-rtc.py script to /usr/local/bin
Installing mm-bolus.py script to /usr/local/bin
Installing mm-set-suspend.py script to /usr/local/bin

Using /usr/local/lib/python2.7/dist-packages/decocare-0.0.18_dev-py2.7.egg
Searching for GitPython==1.0.1
Best match: GitPython 1.0.1
Processing GitPython-1.0.1-py2.7.egg
GitPython 1.0.1 is already the active version in easy-install.pth

Using /usr/local/lib/python2.7/dist-packages/GitPython-1.0.1-py2.7.egg
Searching for argcomplete==1.0.0
Best match: argcomplete 1.0.0
Processing argcomplete-1.0.0-py2.7.egg
argcomplete 1.0.0 is already the active version in easy-install.pth
Installing activate-global-python-argcomplete script to /usr/local/bin
Installing register-python-argcomplete script to /usr/local/bin
Installing python-argcomplete-check-easy-install-script script to /usr/local/bin

Using /usr/local/lib/python2.7/dist-packages/argcomplete-1.0.0-py2.7.egg
Searching for pyserial==2.5
Best match: pyserial 2.5
Adding pyserial 2.5 to easy-install.pth file

Using /usr/lib/python2.7/dist-packages
Searching for gitdb==0.6.4
Best match: gitdb 0.6.4
Processing gitdb-0.6.4-py2.7-linux-armv7l.egg
gitdb 0.6.4 is already the active version in easy-install.pth

Using /usr/local/lib/python2.7/dist-packages/gitdb-0.6.4-py2.7-linux-armv7l.egg
Searching for smmap==0.9.0
Best match: smmap 0.9.0
Processing smmap-0.9.0-py2.7.egg
smmap 0.9.0 is already the active version in easy-install.pth

Using /usr/local/lib/python2.7/dist-packages/smmap-0.9.0-py2.7.egg
Finished processing dependencies for openapscontrib.dose==0.0.0
pi@raspberrypi ~/openaps-dose $ git push
Password for 'https://eszcloud@bitbucket.org':
fatal: Authentication failed
pi@raspberrypi ~/openaps-dose $ git push
Password for 'https://eszcloud@bitbucket.org':
fatal: Authentication failed
pi@raspberrypi ~/openaps-dose $ git push
Password for 'https://eszcloud@bitbucket.org':
fatal: Authentication failed
pi@raspberrypi ~/openaps-dose $ git push
Password for 'https://eszcloud@bitbucket.org':
fatal: Authentication failed
pi@raspberrypi ~/openaps-dose $ git push
Password for 'https://eszcloud@bitbucket.org':
fatal: Authentication failed
pi@raspberrypi ~/openaps-dose $ git push
Password for 'https://eszcloud@bitbucket.org':
fatal: Authentication failed
pi@raspberrypi ~/openaps-dose $ git push
Password for 'https://eszcloud@bitbucket.org':
fatal: Authentication failed
pi@raspberrypi ~/openaps-dose $ cd ..
pi@raspberrypi ~ $ ls
20150920_254pm  20150920_952pm       20150923_311pm  20150924_536pm  bin        openaps-dose  openaps-monitor  typescript
20150920_805pm  20150923_213pm_real  20150924_159pm  20150924_611pm  myopenaps  openaps.ini   python_games
pi@raspberrypi ~ $ cd openaps-
bash: cd: openaps-: No such file or directory
pi@raspberrypi ~ $ cd myopenaps/
pi@raspberrypi ~/myopenaps $ git push
Password for 'https://eszcloud@bitbucket.org':
Counting objects: 590, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (524/524), done.
Writing objects: 100% (579/579), 64.58 KiB, done.
Total 579 (delta 492), reused 0 (delta 0)
To https://eszcloud@bitbucket.org/eszcloud/2015-9-14-openaps-backup.git
   9cd0f9c..a8da443  master -> master
pi@raspberrypi ~/myopenaps $ exit
Script done on Thu 24 Sep 2015 19:51:13 PDT

```




                                                                          [ Read 10 lines ]
^G Get Help                ^O WriteOut                pi@cgmcloud1 ~ $

