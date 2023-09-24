cmake_minimum_required(VERSION 3.5)
set ( TINYGSM_SRC
    "src/TinyGsmBattery.tpp"
    "src/TinyGsmBluetooth.tpp"
    "src/TinyGsmCalling.tpp"
    "src/TinyGsmGPRS.tpp"
    "src/TinyGsmGPS.tpp"
    "src/TinyGsmModem.tpp"
    "src/TinyGsmNTP.tpp"
    "src/TinyGsmSMS.tpp"
    "src/TinyGsmSSL.tpp"
    "src/TinyGsmTCP.tpp"
    "src/TinyGsmTemperature.tpp"
    "src/TinyGsmTime.tpp"
    "src/TinyGsmWifi.tpp"
) 
idf_component_register(SRCS ${TINYGSM_SRC}
                    INCLUDE_DIRS "src/."
                    REQUIRES "arduino" # Library requires Arduino
                    )

project(TinyGSM)