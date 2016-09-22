################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include mbed/TARGET_LPC1768/TOOLCHAIN_GCC_CR/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(CC_DEPS)),)
-include $(CC_DEPS)
endif
ifneq ($(strip $(C++_DEPS)),)
-include $(C++_DEPS)
endif
ifneq ($(strip $(C_UPPER_DEPS)),)
-include $(C_UPPER_DEPS)
endif
ifneq ($(strip $(CXX_DEPS)),)
-include $(CXX_DEPS)
endif
ifneq ($(strip $(CPP_DEPS)),)
-include $(CPP_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: mbed_UART0.axf

# Tool invocations
mbed_UART0.axf: $(OBJS) $(USER_OBJS)
	@echo 'Building target: $@'
	@echo 'Invoking: MCU C++ Linker'
	arm-none-eabi-c++ -nostdlib -L"D:\Dropbox\__Lab Dev\2016_mbed\mbed_UART0" -L"D:\Dropbox\__Lab Dev\2016_mbed\mbed_UART0\mbed" -L"D:\Dropbox\__Lab Dev\2016_mbed\mbed_UART0\mbed\TARGET_LPC1768" -L"D:\Dropbox\__Lab Dev\2016_mbed\mbed_UART0\mbed\TARGET_LPC1768\TARGET_NXP" -L"D:\Dropbox\__Lab Dev\2016_mbed\mbed_UART0\mbed\TARGET_LPC1768\TARGET_NXP\TARGET_LPC176X" -L"D:\Dropbox\__Lab Dev\2016_mbed\mbed_UART0\mbed\TARGET_LPC1768\TARGET_NXP\TARGET_LPC176X\TARGET_MBED_LPC1768" -L"D:\Dropbox\__Lab Dev\2016_mbed\mbed_UART0\mbed\TARGET_LPC1768\TOOLCHAIN_GCC_CR" -Xlinker -Map="mbed_UART0.map" -Xlinker --gc-sections -mcpu=cortex-m3 -mthumb -T "D:\Dropbox\__Lab Dev\2016_mbed\mbed_UART0\mbed\TARGET_LPC1768\TOOLCHAIN_GCC_CR\LPC1768.ld" -o "mbed_UART0.axf" $(OBJS) $(USER_OBJS) $(LIBS)
	@echo 'Finished building target: $@'
	@echo ' '
	$(MAKE) --no-print-directory post-build

# Other Targets
clean:
	-$(RM) $(CC_DEPS)$(C++_DEPS)$(EXECUTABLES)$(C_UPPER_DEPS)$(CXX_DEPS)$(OBJS)$(CPP_DEPS)$(C_DEPS) mbed_UART0.axf
	-@echo ' '

post-build:
	-@echo 'Performing post-build steps'
	-arm-none-eabi-size "mbed_UART0.axf" ; arm-none-eabi-objcopy -O binary "mbed_UART0.axf" "mbed_UART0.bin" ; checksum -p LPC1768 -d "mbed_UART0.bin"
	-@echo ' '

.PHONY: all clean dependents
.SECONDARY: post-build

-include ../makefile.targets
