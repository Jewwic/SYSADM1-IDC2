+----------------------------------+------------------------+----------+
| ![](vertopal_                    |                        |          |
| 8a77c168ae1b4c528a2dcb5acf96ce42 |                        |          |
| /media/image1.png){width="2.4in" |                        |          |
| height="0.5881944444444445in"}   |                        |          |
|                                  |                        |          |
| SCHOOL OF INFORMATION AND        |                        |          |
| TECHNOLOGY                       |                        |          |
+----------------------------------+------------------------+----------+
| NAME: Jerric Panayo              | DATE PERFORMED:        |          |
|                                  | September 12, 2024     |          |
+----------------------------------+------------------------+----------+
| Section: IDC2                    | DATE SUBMITTED:        |          |
|                                  | September 12, 2024     |          |
+----------------------------------+------------------------+----------+

# SYSADM1 -- Managing Services in Linux

# Requirement: 

-   A virtual machine running Linux

![](vertopal_8a77c168ae1b4c528a2dcb5acf96ce42/media/image2.png){width="4.135416666666667in"
height="1.8020833333333333in"}

Complete this lab as follows:

1.  Use the service --status-all command to list all active and inactive
    services.

List down active and inactive services in the table below. Provide five
(5) services for each column.

  -----------------------------------------------------------------------
  **Active**                             **Inactive**
  -------------------------------------- --------------------------------
  cups                                   bluetooth

  cron                                   console-setup.sh

  dbus                                   grub-common

  gdm3                                   keyboard-setup.sh

  kerneloops                             open-vm-tools
  -----------------------------------------------------------------------

SS:

![](vertopal_8a77c168ae1b4c528a2dcb5acf96ce42/media/image3.png){width="5.077073490813648in"
height="4.627866360454943in"}

2.  Start the Bluetooth service using the systemctl command.

Ex. sudo systemctl start httpd

![](vertopal_8a77c168ae1b4c528a2dcb5acf96ce42/media/image4.png){width="4.359946412948381in"
height="1.1875in"}

3.  Check the status of the Bluetooth service. What is its status?

-   The status says enabled but inactive(dead).

SS:

![](vertopal_8a77c168ae1b4c528a2dcb5acf96ce42/media/image5.png){width="6.188086176727909in"
height="4.3345352143482065in"}

1.  Check the status of the cups services. Since when was it running? 25
    minutes ago

SS:
![](vertopal_8a77c168ae1b4c528a2dcb5acf96ce42/media/image6.png){width="5.284647856517935in"
height="3.85002624671916in"}

2.  Stop cups services.

3.  Verify if the service was stopped.

![](vertopal_8a77c168ae1b4c528a2dcb5acf96ce42/media/image7.png){width="7.027083333333334in"
height="3.7131944444444445in"}

4.  Restart the cups services

5.  Verify if the service was restarted.

![](vertopal_8a77c168ae1b4c528a2dcb5acf96ce42/media/image8.png){width="7.027083333333334in"
height="3.7736111111111112in"}
