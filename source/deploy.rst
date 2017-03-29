.. _deploy:

Deploy the code to the RoboRio
==============================

If you are connected to the RoboRio by USB, your IP address is 172.22.11.2. If your are conneted to the wifi
router, your IP address is 10.28.44.26.

The first time you deploy, the script will ask you for the address to the RoboRio. The deploy address is
stored in a local hidden file .deploy_cfg. To update the IP on subsequent deploys, only if you change how you are
connected to the RoboRio.

To deploy your latest changes to the RoboRio, run:

python3 robot.py deploy from the source directory. 