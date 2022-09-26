add_executable(kettle
        kettle.c
        )

# pull in common dependencies
target_link_libraries(kettle pico_stdlib)

# create map/bin/hex file etc.
pico_add_extra_outputs(kettle)

# add url via pico_set_program_url
example_auto_set_url(kettle)