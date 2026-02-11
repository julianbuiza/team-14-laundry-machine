# team-14-laundry-machine
Coin-Operated Laundry Machine, Team 14 for Software Fundamentals 

Team Members:
Julian Buiza 
Evan Helgerman
Caleb Wagner
Madison Werstein
Sneha Chitte
Noor Shsha

A manufacturer is designing a new commercial coin-operated washing machine for laundromats. The manufacturer
wants you to develop an object-oriented software simulator so that they can see whether the machine’s control
logic and coin mechanism will operate reliably and handle the range of customer interactions and fault conditions.
The washing machine offers four wash cycles: quick wash (20 minutes, 2.50 CAD), normal (35 minutes, 3.50
CAD), heavy duty (50 minutes, 4.50 CAD), and delicate (30 minutes, 3.00 CAD). Each cycle consists of a fixed
sequence of phases: fill, wash, drain, rinse, drain, and spin. The duration and motor speed of each phase varies by
cycle.
The machine has a hot water valve, a cold water valve, a drum motor with three speeds (low, medium, high), a
drain pump, and a solenoid-operated door latch. The machine operates in two modes, depending on whether or
not a technician key is inserted into the control panel.
In customer mode, the customer loads clothes, closes the door (which latches automatically), selects a cycle using
a rotary dial, selects a water temperature (hot, warm, or cold), and inserts coins. The machine accepts 25cent,
1 CAD, and 2 CAD coins. A small display shows the remaining balance needed. Once full payment is received,
the start button become enabled. Pressing start begins the cycle and the door locks, it cannot be opened until the
cycle is complete and the drum has fully stopped. If the customer opens the door before paying, the coins already
inserted remain credited for 2 minutes before being returned internally to the coin return cup.
When the technician key is inserted, the machine enters diagnostic mode and the current cycle, if any, is paused.
In this mode it is possible:
1. to run each component independently (fill hot, fill cold, drain, spin at each speed);
2. to empty the coin box;
3. to set the pricing for each cycle;
4. to view error logs and lifetime cycle counts;
5. to remove the key and return to customer mode (resuming any paused cycle).
The machine has sensors for water level (low, medium, high), drum speed, water temperature, door position (open
or closed), and vibration. If the vibration sensor detects an unbalanced load during the spin phase, the machine
stops the drum, runs a low-speed tumble for 30 seconds to redistribute the load, and retries the spin. It will retry up
to three times before halting the cycle and displaying an error code. The drain can occasionally clog, in which case
the water level sensor will not drop during the drain phase within the expected time; the machine must detect this,
halt, and display an error. Approximately 4% of cycles experience an unbalanced load event, and approximately
1% experience a drain clog.
Your simulation should allow the user to either directly control the events that happen or enter an automatic
mode where customers arrive and use the machine randomly throughout a simulated day. It should be able to
help answer questions such as how much revenue the machine generates per day, how often the unbalanced-load
retry succeeds versus requiring a technician, and how the fault rates affect machine availability over a week of
continuous operation. In order to do this your simulation needs to keep statistics as it runs and print them out on
request, and needs to use random number generators to simulate customer behaviour and mechanical faults.
8
7
1. to run each component independently (fill hot, fill cold, drain, spin at each speed);
2. to empty the coin box;
3. to set the pricing for each cycle;
4. to view error logs and lifetime cycle counts;
5. to remove the key and return to customer mode (resuming any paused cycle).
