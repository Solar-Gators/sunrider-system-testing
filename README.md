# Sunrider System Testing

## Install Renode

- Download and install Renode [using their instructions](https://github.com/renode/renode/blob/master/README.rst#installation)

## Running the Automated Tests

Renode is integrated [with the Robot Framework for testing](https://renode.readthedocs.io/en/latest/introduction/testing.html). To run the test use the following command:

```bash
    renode-test my_test.robot
```

## Running the Sim Manually

To run the simulation manually run the following command:

```bash
renode -e s mystm.repl
```

This will start Renode in a different window. [See their documentation](https://renode.readthedocs.io/en/latest/basic/machines.html) for how to interact with machines.

## Changing the Source

- Pull my branch [rbernardo/renode](https://github.com/John-Carr/TelemetryFirmware/tree/rbernardo/renode)

- Build the code in STM32Cube

- Copy the .elf file from the Debug/{PROJECT_NAME}.elf to the directory of this project

- Rename the .elf to OpenTelemetry.elf
