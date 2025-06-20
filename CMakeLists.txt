add_library(grbl INTERFACE)

target_include_directories(grbl INTERFACE
    $<BUILD_INTERFACE:${CMAKE_CURRENT_LIST_DIR}>
)

target_sources(grbl INTERFACE
 ${CMAKE_CURRENT_LIST_DIR}/grbllib.c
 ${CMAKE_CURRENT_LIST_DIR}/coolant_control.c
 ${CMAKE_CURRENT_LIST_DIR}/crossbar.c
 ${CMAKE_CURRENT_LIST_DIR}/crc.c
 ${CMAKE_CURRENT_LIST_DIR}/nvs_buffer.c
 ${CMAKE_CURRENT_LIST_DIR}/gcode.c
 ${CMAKE_CURRENT_LIST_DIR}/machine_limits.c
 ${CMAKE_CURRENT_LIST_DIR}/messages.c
 ${CMAKE_CURRENT_LIST_DIR}/modbus.c
 ${CMAKE_CURRENT_LIST_DIR}/modbus_rtu.c
 ${CMAKE_CURRENT_LIST_DIR}/motion_control.c
 ${CMAKE_CURRENT_LIST_DIR}/my_plugin.c
 ${CMAKE_CURRENT_LIST_DIR}/nuts_bolts.c
 ${CMAKE_CURRENT_LIST_DIR}/override.c
 ${CMAKE_CURRENT_LIST_DIR}/planner.c
 ${CMAKE_CURRENT_LIST_DIR}/protocol.c
 ${CMAKE_CURRENT_LIST_DIR}/report.c
 ${CMAKE_CURRENT_LIST_DIR}/settings.c
 ${CMAKE_CURRENT_LIST_DIR}/sleep.c
 ${CMAKE_CURRENT_LIST_DIR}/spindle_control.c
 ${CMAKE_CURRENT_LIST_DIR}/state_machine.c
 ${CMAKE_CURRENT_LIST_DIR}/stream.c
 ${CMAKE_CURRENT_LIST_DIR}/stream_file.c
 ${CMAKE_CURRENT_LIST_DIR}/stream_passthru.c
 ${CMAKE_CURRENT_LIST_DIR}/stepper.c
 ${CMAKE_CURRENT_LIST_DIR}/stepper2.c
 ${CMAKE_CURRENT_LIST_DIR}/strutils.c
 ${CMAKE_CURRENT_LIST_DIR}/system.c
 ${CMAKE_CURRENT_LIST_DIR}/tool_change.c
 ${CMAKE_CURRENT_LIST_DIR}/alarms.c
 ${CMAKE_CURRENT_LIST_DIR}/errors.c
 ${CMAKE_CURRENT_LIST_DIR}/ngc_params.c
 ${CMAKE_CURRENT_LIST_DIR}/ngc_expr.c
 ${CMAKE_CURRENT_LIST_DIR}/ngc_flowctrl.c
 ${CMAKE_CURRENT_LIST_DIR}/regex.c
 ${CMAKE_CURRENT_LIST_DIR}/ioports.c
 ${CMAKE_CURRENT_LIST_DIR}/vfs.c
 ${CMAKE_CURRENT_LIST_DIR}/canbus.c
 ${CMAKE_CURRENT_LIST_DIR}/pid.c
 ${CMAKE_CURRENT_LIST_DIR}/kinematics/corexy.c
 ${CMAKE_CURRENT_LIST_DIR}/kinematics/wall_plotter.c
 ${CMAKE_CURRENT_LIST_DIR}/kinematics/delta.c
 ${CMAKE_CURRENT_LIST_DIR}/kinematics/polar.c
)
