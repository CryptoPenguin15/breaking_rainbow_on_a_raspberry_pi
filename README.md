# Breaking Rainbow on a Raspberry Pi

Documentation to get started and run the toy example from start to finish.

## HW
[Raspberry Pi](https://www.raspberrypi.com/)

## Prereq

According to the two repos dependencies.

## Build

The following instructions assume the repositories are cloned with xl within the BreakingRainbow repo.

Clone
[BreakingRainbow](https://github.com/WardBeullens/BreakingRainbow)

```sh
cd BreakingRainbow
```

Clone
[xl](https://github.com/CryptoPenguin15/xl)

```sh
cd xl
```

Verify the xl setup using the two available test suites. Some distros lack the NUMA headers. In that case, disable NUMA support in the xl Makefile.

Configure the Makefile with
```sh
Q = 16
M = 43
N = 20
```

```sh
cd ../Attack_demo
```

Edit `Full_Attack.sage` and replace `/xl-20160426` with `/xl`.

## Run demo

- Generate a keypair
- Run the secret key recovery script

---

## Disclaimer
The Round 2 SL 1 parameters will have the Pi running for days. All four cores are utilised at 95%-100%. Temperatures, using standard fan cooling, reach 77-80 degrees Celsius, (Raspberry Pi5, 8GB). Use at own risk.

## License
This project is licensed under the MIT License.
See [LICENSE](LICENSE) for details.
