Ansible Role to install and configure Universal Media Server 
=============================================================

Application HomePage: http://www.universalmediaserver.com/

--------------------------------------------------------

Check defaults/[main.yaml](defaults/main.yml) for default settings and playbook example.


example playbook variables-
--------------------------------------------------------
```
ums_version: "6.7.3"
ums_remote_source: "http://home.rabd.co.uk/downloads/UMS-6.7.3.tgz"
ums_server_name: Dmedia

ums_folder_config:
  - setting: folders
    value: "/media/dmedia/Shared,/media/apps"

ums_max_config:
  - setting: hide_empty_folders
    value: true
  - setting: hide_transcode_folder
    value: true
  - setting: hide_recently_played_folder
    value: true
  - setting: gpu_acceleration
    value: true
  - setting: disable_subtitles
    value: true
  - setting: resume
    value: false
```
^^
# Keep adding here for more settings.
# List of avaiable settgins can be found in original config file in templates/ [UMS.conf_orig.j2](templates/UMS.conf_orig.j2)

#

Dependencies-
--------------------------------------------------------
None

Author-
--------------------------------------------------------

Rabbi Ahmed

