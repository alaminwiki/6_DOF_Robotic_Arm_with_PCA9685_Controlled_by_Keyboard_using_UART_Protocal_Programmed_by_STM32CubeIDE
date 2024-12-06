################################################################################
# Automatically-generated file. Do not edit!
# Toolchain: GNU Tools for STM32 (12.3.rel1)
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include Drivers/STM32F1xx_HAL_Driver/Src/subdir.mk
-include Core/Startup/subdir.mk
-include Core/Src/subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(S_DEPS)),)
-include $(S_DEPS)
endif
ifneq ($(strip $(S_UPPER_DEPS)),)
-include $(S_UPPER_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

OPTIONAL_TOOL_DEPS := \
$(wildcard ../makefile.defs) \
$(wildcard ../makefile.init) \
$(wildcard ../makefile.targets) \


BUILD_ARTIFACT_NAME := 6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx
BUILD_ARTIFACT_EXTENSION := elf
BUILD_ARTIFACT_PREFIX :=
BUILD_ARTIFACT := $(BUILD_ARTIFACT_PREFIX)$(BUILD_ARTIFACT_NAME)$(if $(BUILD_ARTIFACT_EXTENSION),.$(BUILD_ARTIFACT_EXTENSION),)

# Add inputs and outputs from these tool invocations to the build variables 
EXECUTABLES += \
6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.elf \

MAP_FILES += \
6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.map \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.list \

OBJCOPY_HEX += \
6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.hex \

OBJCOPY_BIN += \
6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.bin \


# All Target
all: main-build

# Main-build Target
main-build: 6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.elf secondary-outputs

# Tool invocations
6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.elf 6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.map: $(OBJS) $(USER_OBJS) D:\LK\ Sir\ batch\ \ 242\242_EEE_3403_Lecture10\Serial_Tx_Rx\Serial_Tx_Rx\STM32F103C8TX_FLASH.ld makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-gcc -o "6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m3 -T"D:\LK Sir batch  242\242_EEE_3403_Lecture10\Serial_Tx_Rx\Serial_Tx_Rx\STM32F103C8TX_FLASH.ld" --specs=nosys.specs -Wl,-Map="6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.map" -Wl,--gc-sections -static --specs=nano.specs -mfloat-abi=soft -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES) makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.list: $(EXECUTABLES) makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.list"
	@echo 'Finished building: $@'
	@echo ' '

6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.hex: $(EXECUTABLES) makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-objcopy  -O ihex $(EXECUTABLES) "6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.hex"
	@echo 'Finished building: $@'
	@echo ' '

6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.bin: $(EXECUTABLES) makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-objcopy  -O binary $(EXECUTABLES) "6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.bin"
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) 6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.bin 6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.elf 6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.hex 6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.list 6_DOF_Robotic_Arm_With_PCA9685_Controll_with_keyboard_by_Serial_Tx_Rx.map default.size.stdout
	-@echo ' '

secondary-outputs: $(SIZE_OUTPUT) $(OBJDUMP_LIST) $(OBJCOPY_HEX) $(OBJCOPY_BIN)

fail-specified-linker-script-missing:
	@echo 'Error: Cannot find the specified linker script. Check the linker settings in the build configuration.'
	@exit 2

warn-no-linker-script-specified:
	@echo 'Warning: No linker script specified. Check the linker settings in the build configuration.'

.PHONY: all clean dependents main-build fail-specified-linker-script-missing warn-no-linker-script-specified

-include ../makefile.targets
