# ANN on Arduino

At least **6KB RAM** is required, or you'll need to trim training dataset, or use smaller network.

Currently I'm using 150 training samples from Iris dataset to train a neural network with one hidden layer, 4 inputs, 4 hidden nodes for each hidden layer, and 3 outputs.

| MCU            | Frequency | FLASH  | RAM   | Train Time | Pred Time | Accuracy |
| -------------- | --------- | ------ | ----- | ---------- | --------- | -------- |
| STM32F429IGT6  | 180MHz    | 1024KB | 256KB | 9s         | 7ms       | 96.0%    |
| STM32F401RET6  | 84MHz     | 512KB  | 96KB  | 18s        | 15ms      | 96.0%    |
| STM32L475VET6  | 80MHz     | 512KB  | 128KB | 24s        | 22ms      | 96.0%    |
| STM32F103RCT6  | 72MHz     | 256KB  | 20KB  | 32s        | 26ms      | 96.0%    |
| STM32F103C8T6  | 72MHz     | 64KB   | 20KB  | 32s        | 26ms      | 96.0%    |
| Arduino M0 Pro | 48MHz     | 256KB  | 32KB  | 135s       | 97ms      | 96.0%    |
| ATmega 2560    | 16MHz     | 256KB  | 8KB   | 182s       | 138ms     | 96.0%    |

## Related Projects

- codeplea: https://github.com/codeplea/genann

- wuhanstudio: https://github.com/wuhanstudio/rt-libann

## Contact

* Author：Wu Han
* Home：http://wuhanstudio.cc
* Contact：https://github.com/wuhanstudio/arduino_ann/issues
