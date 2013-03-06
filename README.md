#ATM

## Package
The main Namespace is com.progress.demo.rce.atm

## Events
* **NewATM**(integer id). It defines a new ATM machine thay will recieve movements made by the simulator.
* **NewSim**(integer id, float limX, float limY). It defines a new ATM operations simulator.
* **Activity**(integer id, integer card, float amount, string currency). Pay event that includes the terminal id where it was made, a random card number, a random amount and the pay currency.
* **Stream**(string channel, integer idChannel, integer idClient, sequence<string> extra). The output event that has the information about the channel, its id, the client id and the extra information.
In this case, the channel is "ATM", its id corresponds to the machine number, the client id is defined by the card number, and extra = [amount, currency].


