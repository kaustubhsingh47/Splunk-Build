Bash script "ecsl_system_builder.sh" used to build the file system structure for the "ecsl" application, with some additional settings and configurations for Splunk-TI usage.

The script is using Bash shell to run. It contains a number of functions such as lecho(), setAppDirs(), makeAppDirs(), makelinks(), which perform various tasks.

The script first checks if the user running the script is the root user, and if not, exits with an error message. Then, it defines several variables related to the application directory structure such as corpDir, topDir, aitDir, appDir, etcDir, panDir, scrDir, dataDir, and localDir. These variables are used in the later functions to create and set permissions for various directories.

The makeAppDirs() function creates the required directories for the application, sets permissions, and creates symbolic links. The makelinks() function creates symbolic links for directories such as /data, /data/ecsinas, /data/logspool, and /data/syslog.

The script also checks for Splunk-TI usage and creates a symbolic link for the splunk directory.
