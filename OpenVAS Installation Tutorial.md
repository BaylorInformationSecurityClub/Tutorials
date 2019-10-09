OpenVAS Installation Tutorial

1.  Open Terminal and run the following

    1.  apt-get install openvas

    2.  openvas-setup

    3.  netstat -antp

    4.  openvas-start

        1.  Run if browser does not automatically pop up or you are rebooting
            machine

2.  Open <https://127.0.0.1:9392> in the browser

3.  Login and you are done!

    1.  Login is displayed at the end of the install

4.  If you get an error in the web interface saying something about there not
    being a database, run the following commands in terminal. This manually
    syncs the databases and restarts the services.

    1.  greenbone-nvt-sync

    2.  greenbone-scapdata-sync

    3.  greenbone-certdata-sync

    4.  systemctl restart openvas-scanner

    5.  systemctl restart openvas-manager

    6.  systemctl restart openvas-gsa

5.  If you want to set openvas services to start on boot, enter the following
    commands

    1.  systemctl enable openvas-scanner

    2.  systemctl enable openvas-manager

    3.  systemctl enable openvas-gsa

6.  Still getting errors in the user interface?

    1.  openvas-check-setup
