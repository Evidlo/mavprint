# mavprint

Print mavlink messages to console

## Quickstart

    pip install mavprint
    mavprint --port /dev/ttyACM1 show

## Examples

    # show all messages except BAD_DATA
    $ mavprint show --exclude BAD_DATA
    SERVO_OUTPUT_RAW {time_usec : 4069392862, port : 0, servo1_raw : 900, servo2_raw : 900, servo3_raw : 900, servo4_raw : 900, servo5_raw : 0, servo6_raw : 0, servo7_raw : 0, servo8_raw : 0}
    ATTITUDE {time_boot_ms : 8364376, roll : 0.21510164439678192, pitch : 0.04040948674082756, yaw : -2.9597930908203125, rollspeed : -0.004067523404955864, pitchspeed : 0.0025288478937000036, yawspeed : 0.0004264041199348867}
    ...

    # show number of messages of each type captured while running
    $ mavprint unique
    ^C
    {   'ACTUATOR_CONTROL_TARGET': 34,
        'ALTITUDE': 11,
        'ATTITUDE': 56,
        'ATTITUDE_QUATERNION': 57,
        'ATTITUDE_TARGET': 10,
        'BAD_DATA': 4,
        'BATTERY_STATUS': 1,
        'ESTIMATOR_STATUS': 6,
        'EXTENDED_SYS_STATE': 3,
        'HEARTBEAT': 2,
        'HIGHRES_IMU': 57,
        'LOCAL_POSITION_NED': 35,
        'PING': 2,
        'SCALED_IMU': 29,
        'SCALED_IMU2': 29,
        'SERVO_OUTPUT_RAW': 22,
        'SYS_STATUS': 2,
        'TIMESYNC': 12,
        'VFR_HUD': 22,
        'VIBRATION': 3}
