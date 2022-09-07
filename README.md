# Building

    mkdir build
    cd build
    cmake ..
    make install # This may require sudo

## Updating world file

    cd worlds
    erb simple_city.world.erb > simple_city.world


# Running

1. Source setup file

    . [install_prefix]/share/citysim/setup.sh  
    #### For Example:  
    . source /usr/local/share/citysim-0/setup.sh


1. Open world

    gazebo worlds/simple_city.world


