## To create a map.

You need the bag file: test_robotnik_rslidar_09-05-2019_garage.bag, from RBKairos

Launch in two terminals:

``` roslaunch rbares_localization_3d slam_complete.launch visualization:=true ```

``` roslaunch rbares_localization_3d play_robotnik.launch ```

## To localize.


``` roslaunch rbares_localization_3d localization_complete.launch visualization:=true ```

``` roslaunch rbares_localization_3d play_robotnik.launch ```

## Notes

Check that map is not published by play_robotnik when SLAM is being done.

If scan_registration and mcl3_3dl complain about extrapolation to the past, play the bag file before running the nodes.
