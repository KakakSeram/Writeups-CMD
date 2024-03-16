# Mount Shared Folder

Mount Shared Folder Linux on VMware

* Set shared folder on VMware properties

    ![sharedfoldervmware.png](./images/sharedfoldervmware.png)

* Check VMware share folder

    `vmware-hgfsclient`

    ![hgfsclient](./images/hgfsclient.png)

*  Mount folder

    `sudo vmhgfs-fuse .host:/ /mnt/hgfs/ -o allow_other -o uid=1000`

    ![mount-hgfsclient](./images/mount-hgfsclient.png)
