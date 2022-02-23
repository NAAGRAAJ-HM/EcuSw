cmake_minimum_required(VERSION 3.16.3)

project(
   EcuSw.out
   VERSION 0.1
)

SET(CMAKE_CXX_STANDARD 14)
SET(CMAKE_CXX_STANDARD_REQUIRED True)

add_definitions(
   -g
   -std=c++14
   -Wall
   -Werror
   -Wextra
   -pedantic
   -Wuninitialized
)

add_executable(
   EcuSw.out
   ./Rte/LATEST/Rte.cpp
   ./SwcApplFoc/LATEST/SwcApplFoc.cpp
)

add_subdirectory(BswAUTOSAR_EcuAb_CanIf/LATEST     BswAUTOSAR_EcuAb_CanIf/LATEST)
add_subdirectory(BswAUTOSAR_EcuAb_CryIf/LATEST     BswAUTOSAR_EcuAb_CryIf/LATEST)
add_subdirectory(BswAUTOSAR_EcuAb_Ea/LATEST        BswAUTOSAR_EcuAb_Ea/LATEST)
add_subdirectory(BswAUTOSAR_EcuAb_EthIf/LATEST     BswAUTOSAR_EcuAb_EthIf/LATEST)
add_subdirectory(BswAUTOSAR_EcuAb_Fee/LATEST       BswAUTOSAR_EcuAb_Fee/LATEST)
add_subdirectory(BswAUTOSAR_EcuAb_FrIf/LATEST      BswAUTOSAR_EcuAb_FrIf/LATEST)
add_subdirectory(BswAUTOSAR_EcuAb_LinIf/LATEST     BswAUTOSAR_EcuAb_LinIf/LATEST)
add_subdirectory(BswAUTOSAR_EcuAb_LinTp/LATEST     BswAUTOSAR_EcuAb_LinTp/LATEST)
add_subdirectory(BswAUTOSAR_EcuAb_MemIf/LATEST     BswAUTOSAR_EcuAb_MemIf/LATEST)
add_subdirectory(BswAUTOSAR_EcuAb_WdgIf/LATEST     BswAUTOSAR_EcuAb_WdgIf/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Adc/LATEST        BswAUTOSAR_McAL_Adc/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Can/LATEST        BswAUTOSAR_McAL_Can/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Cry/LATEST        BswAUTOSAR_McAL_Cry/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Dio/LATEST        BswAUTOSAR_McAL_Dio/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Eep/LATEST        BswAUTOSAR_McAL_Eep/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Eth/LATEST        BswAUTOSAR_McAL_Eth/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Fls/LATEST        BswAUTOSAR_McAL_Fls/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Fr/LATEST         BswAUTOSAR_McAL_Fr/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Gpt/LATEST        BswAUTOSAR_McAL_Gpt/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Icu/LATEST        BswAUTOSAR_McAL_Icu/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Lin/LATEST        BswAUTOSAR_McAL_Lin/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Mcu/LATEST        BswAUTOSAR_McAL_Mcu/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Ocu/LATEST        BswAUTOSAR_McAL_Ocu/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Port/LATEST       BswAUTOSAR_McAL_Port/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Pwm/LATEST        BswAUTOSAR_McAL_Pwm/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Spi/LATEST        BswAUTOSAR_McAL_Spi/LATEST)
add_subdirectory(BswAUTOSAR_McAL_Wdg/LATEST        BswAUTOSAR_McAL_Wdg/LATEST)
add_subdirectory(BswAUTOSAR_Service_BswM/LATEST    BswAUTOSAR_Service_BswM/LATEST)
add_subdirectory(BswAUTOSAR_Service_Com/LATEST     BswAUTOSAR_Service_Com/LATEST)
add_subdirectory(BswAUTOSAR_Service_ComM/LATEST    BswAUTOSAR_Service_ComM/LATEST)
add_subdirectory(BswAUTOSAR_Service_Csm/LATEST     BswAUTOSAR_Service_Csm/LATEST)
add_subdirectory(BswAUTOSAR_Service_Dcm/LATEST     BswAUTOSAR_Service_Dcm/LATEST)
add_subdirectory(BswAUTOSAR_Service_Dem/LATEST     BswAUTOSAR_Service_Dem/LATEST)
add_subdirectory(BswAUTOSAR_Service_Det/LATEST     BswAUTOSAR_Service_Det/LATEST)
add_subdirectory(BswAUTOSAR_Service_EcuM/LATEST    BswAUTOSAR_Service_EcuM/LATEST)
add_subdirectory(BswAUTOSAR_Service_FiM/LATEST     BswAUTOSAR_Service_FiM/LATEST)
add_subdirectory(BswAUTOSAR_Service_Nm/LATEST      BswAUTOSAR_Service_Nm/LATEST)
add_subdirectory(BswAUTOSAR_Service_NvM/LATEST     BswAUTOSAR_Service_NvM/LATEST)
add_subdirectory(BswAUTOSAR_Service_Os/LATEST      BswAUTOSAR_Service_Os/LATEST)
add_subdirectory(BswAUTOSAR_Service_PduR/LATEST    BswAUTOSAR_Service_PduR/LATEST)
add_subdirectory(BswAUTOSAR_Service_SchM/LATEST    BswAUTOSAR_Service_SchM/LATEST)
add_subdirectory(BswAUTOSAR_Service_SecOC/LATEST   BswAUTOSAR_Service_SecOC/LATEST)
add_subdirectory(BswAUTOSAR_Service_SokFm/LATEST   BswAUTOSAR_Service_SokFm/LATEST)
add_subdirectory(BswAUTOSAR_Service_StartUp/LATEST BswAUTOSAR_Service_StartUp/LATEST)
add_subdirectory(BswAUTOSAR_Service_StbM/LATEST    BswAUTOSAR_Service_StbM/LATEST)
add_subdirectory(BswAUTOSAR_Service_Vkms/LATEST    BswAUTOSAR_Service_Vkms/LATEST)
add_subdirectory(BswAUTOSAR_Service_WdgM/LATEST    BswAUTOSAR_Service_WdgM/LATEST)
add_subdirectory(SwcServiceEcuM/LATEST             SwcServiceEcuM/LATEST)
add_subdirectory(SwcServiceOs/LATEST               SwcServiceOs/LATEST)

target_link_libraries(
   EcuSw.out PUBLIC
   BswAUTOSAR_EcuAb_CanIf
   BswAUTOSAR_EcuAb_CryIf
   BswAUTOSAR_EcuAb_Ea
   BswAUTOSAR_EcuAb_EthIf
   BswAUTOSAR_EcuAb_Fee
   BswAUTOSAR_EcuAb_FrIf
   BswAUTOSAR_EcuAb_LinIf
   BswAUTOSAR_EcuAb_LinTp
   BswAUTOSAR_EcuAb_MemIf
   BswAUTOSAR_EcuAb_WdgIf
   BswAUTOSAR_McAL_Adc
   BswAUTOSAR_McAL_Can
   BswAUTOSAR_McAL_Cry
   BswAUTOSAR_McAL_Dio
   BswAUTOSAR_McAL_Eep
   BswAUTOSAR_McAL_Eth
   BswAUTOSAR_McAL_Fls
   BswAUTOSAR_McAL_Fr
   BswAUTOSAR_McAL_Gpt
   BswAUTOSAR_McAL_Icu
   BswAUTOSAR_McAL_Lin
   BswAUTOSAR_McAL_Mcu
   BswAUTOSAR_McAL_Ocu
   BswAUTOSAR_McAL_Port
   BswAUTOSAR_McAL_Pwm
   BswAUTOSAR_McAL_Spi
   BswAUTOSAR_McAL_Wdg
   BswAUTOSAR_Service_BswM
   BswAUTOSAR_Service_Com
   BswAUTOSAR_Service_ComM
   BswAUTOSAR_Service_Csm
   BswAUTOSAR_Service_Dcm
   BswAUTOSAR_Service_Dem
   BswAUTOSAR_Service_Det
   BswAUTOSAR_Service_EcuM
   BswAUTOSAR_Service_FiM
   BswAUTOSAR_Service_Nm
   BswAUTOSAR_Service_NvM
   BswAUTOSAR_Service_Os
   BswAUTOSAR_Service_PduR
   BswAUTOSAR_Service_SchM
   BswAUTOSAR_Service_SecOC
   BswAUTOSAR_Service_SokFm
   BswAUTOSAR_Service_StartUp
   BswAUTOSAR_Service_StbM
   BswAUTOSAR_Service_Vkms
   BswAUTOSAR_Service_WdgM
   SwcServiceEcuM
   SwcServiceOs
)

target_include_directories(
   EcuSw.out PUBLIC
   "${PROJECT_BINARY_DIR}"
   "${PROJECT_SOURCE_DIR}/Rte/LATEST"
   "${PROJECT_SOURCE_DIR}/Swc_Foc/LATEST"
)

