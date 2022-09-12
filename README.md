# Building

    mkdir build
    cd build
    cmake ..
    make install # This may require sudo


# Running

1. Source setup file

    . [install_prefix]/share/citysim/setup.sh  
    #### For Example:  
    `source /usr/local/share/citysim-0/setup.sh`

1. Open world to test if it is working.   
- The first time running this may take a long time and then fail. If so close gazebosim and reopen and it will typically work from now on.  
- The cause of this is related to Gazebo needing to download resources that it does not yet have and this world model uses a lot of models that need downloading.
- Most error messages of the sort 'Error [parser.cc:749] Could not find model.config or manifest.xml in [/usr/share//gazebo]' can be ignored.

    gazebo worlds/simple_city.world

## Updating world file

    cd worlds
    erb simple_city.world.erb > simple_city.world