################################################################################
# Automatically-generated file. Do not edit!
################################################################################

SHELL = cmd.exe

CG_TOOL_ROOT := D:/Program Files (x86)/msp430_4.2.1

ORDERED_OBJS += \
$(GEN_CMDS__FLAG) \
"./libraries/NCN_GPIO.obj" \
"./tmain.obj" \
"./t_my_app.obj" \
-l"D:\GitHub\np-public-sw-firmware-msp430g2553-modules\Click&PLAY project\20160607-1051\Click&PLAY\mdk\np_module_mdk_v1.lib" \
-l"libc.a" \
"../lnk_msp430g2553.cmd" \
"../mdk/np_module_mdk_v1.lib" \

-include ../makefile.init

RM := DEL /F
RMDIR := RMDIR /S/Q

# All of the sources participating in the build are defined here
-include sources.mk
-include subdir_vars.mk
-include mdk/subdir_vars.mk
-include libraries/subdir_vars.mk
-include subdir_rules.mk
-include mdk/subdir_rules.mk
-include libraries/subdir_rules.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(S_DEPS)),)
-include $(S_DEPS)
endif
ifneq ($(strip $(S_UPPER_DEPS)),)
-include $(S_UPPER_DEPS)
endif
ifneq ($(strip $(S62_DEPS)),)
-include $(S62_DEPS)
endif
ifneq ($(strip $(C64_DEPS)),)
-include $(C64_DEPS)
endif
ifneq ($(strip $(ASM_DEPS)),)
-include $(ASM_DEPS)
endif
ifneq ($(strip $(CC_DEPS)),)
-include $(CC_DEPS)
endif
ifneq ($(strip $(S55_DEPS)),)
-include $(S55_DEPS)
endif
ifneq ($(strip $(C67_DEPS)),)
-include $(C67_DEPS)
endif
ifneq ($(strip $(C??_DEPS)),)
-include $(C??_DEPS)
endif
ifneq ($(strip $(CLA_DEPS)),)
-include $(CLA_DEPS)
endif
ifneq ($(strip $(CPP_DEPS)),)
-include $(CPP_DEPS)
endif
ifneq ($(strip $(S??_DEPS)),)
-include $(S??_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
ifneq ($(strip $(C62_DEPS)),)
-include $(C62_DEPS)
endif
ifneq ($(strip $(CXX_DEPS)),)
-include $(CXX_DEPS)
endif
ifneq ($(strip $(C++_DEPS)),)
-include $(C++_DEPS)
endif
ifneq ($(strip $(ASM_UPPER_DEPS)),)
-include $(ASM_UPPER_DEPS)
endif
ifneq ($(strip $(K_DEPS)),)
-include $(K_DEPS)
endif
ifneq ($(strip $(C43_DEPS)),)
-include $(C43_DEPS)
endif
ifneq ($(strip $(S67_DEPS)),)
-include $(S67_DEPS)
endif
ifneq ($(strip $(SA_DEPS)),)
-include $(SA_DEPS)
endif
ifneq ($(strip $(S43_DEPS)),)
-include $(S43_DEPS)
endif
ifneq ($(strip $(OPT_DEPS)),)
-include $(OPT_DEPS)
endif
ifneq ($(strip $(S64_DEPS)),)
-include $(S64_DEPS)
endif
ifneq ($(strip $(C_UPPER_DEPS)),)
-include $(C_UPPER_DEPS)
endif
ifneq ($(strip $(C55_DEPS)),)
-include $(C55_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: Click_PLAY.out

# Tool invocations
Click_PLAY.out: $(OBJS) $(CMD_SRCS) $(LIB_SRCS) $(GEN_CMDS)
	@echo 'Building target: $@'
	@echo 'Invoking: MSP430 Linker'
	"D:/Program Files (x86)/msp430_4.2.1/bin/cl430" -vmsp --abi=eabi --advice:power="all" -g --define=__MSP430G2553__ --diag_warning=225 --display_error_number --diag_wrap=off --printf_support=minimal -z -m"Click_PLAY.map" --heap_size=80 --stack_size=80 -i"D:/CCS5.3.0/ccsv5/ccs_base/msp430/include" -i"D:/GitHub/np-public-sw-firmware-msp430g2553-modules/Click&PLAY project/20160607-1051/Click&PLAY/mdk" -i"D:/GitHub/np-public-sw-firmware-msp430g2553-modules/Click&PLAY project/20160607-1051/Click&PLAY" -i"D:/GitHub/np-public-sw-firmware-msp430g2553-modules/Click&PLAY project/20160607-1051/Click&PLAY/libraries" -i"D:/Program Files (x86)/msp430_4.2.1/lib" -i"D:/Program Files (x86)/msp430_4.2.1/include" --reread_libs --warn_sections --display_error_number --diag_wrap=off --xml_link_info="Click_PLAY_linkInfo.xml" --rom_model -o "Click_PLAY.out" $(ORDERED_OBJS)
	@echo 'Finished building target: $@'
	@echo ' '
	$(MAKE) --no-print-directory post-build

# Other Targets
clean:
	-$(RM) $(MSP430_EXECUTABLE_OUTPUTS__QUOTED) "Click_PLAY.out"
	-$(RM) "tmain.pp" 
	-$(RM) "t_my_app.pp" "libraries\NCN_GPIO.pp" 
	-$(RM) "t_my_app.obj" "tmain.obj" "libraries\NCN_GPIO.obj" 
	-@echo 'Finished clean'
	-@echo ' '

post-build:
	-@echo 'Create flash image: TI-TXT'
	-"D:/Program Files (x86)/msp430_4.2.1/bin/hex430" --ti_txt "Click_PLAY.out" -o "Click_PLAY.txt" -order MS -romwidth 16
	-@echo ' '

.PHONY: all clean dependents
.SECONDARY: post-build

-include ../makefile.targets
