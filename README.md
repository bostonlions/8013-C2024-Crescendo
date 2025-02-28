C2024
--
![324946203-191848ec-dabc-4496-be2c-9f4f57d91866](https://github.com/user-attachments/assets/18054805-b7c8-4c0d-823a-697da49e66d6)

Code for Team 8013's 2024 robot, Crepe Flipper.

----------------------------------------------------------

**Highlights:**
- Field-Relative Swerve Drive
- Multi Game Piece Autonomous Modes going up to 4 pieces.
- Trap Climb Sequence in under 6 seconds
- Able to do every task: Shoot, Amp, Trap
- Code implemented from 1678 Citrus Circuts, 5940 Bread, and 2910 Jack in the Bot

**Major Package Functions:**

- [com.team8013.frc2024](https://github.com/maxconine/8013-2024-Crescendo-Imported-v2/tree/Public-Code-2024/src/main/java/com/team8013/frc2024)

  Contains central robot functions specific to Crepe Flipper. Robot control originates from the Robot class.

- [com.team8013.frc2024.auto](https://github.com/maxconine/8013-2024-Crescendo-Imported-v2/tree/Public-Code-2024/src/main/java/com/team8013/frc2024/auto)

  Handles generation, selection, and execution of autonomous routines.

- [com.team8013.frc2024.auto.actions](https://github.com/maxconine/8013-2024-Crescendo-Imported-v2/tree/Public-Code-2024/src/main/java/com/team8013/frc2024/auto/actions)

  Contains all actions used during autonomous. All actions must implement the Action interface.

- [com.team8013.frc2024.auto.modes](https://github.com/maxconine/8013-2024-Crescendo-Imported-v2/tree/Public-Code-2024/src/main/java/com/team8013/frc2024/auto/modes)

  Contains all autonomous modes. These modes are selected in com.team8013.frc2024.auto.AutoModeSelector

- [com.team8013.frc2024.controlboard](https://github.com/maxconine/8013-2024-Crescendo-Imported-v2/tree/Public-Code-2024/src/main/java/com/team8013/frc2024/controlboard)

  Handles polling driver and operator inputs from one [`Xbox Controller`](src/main/java/com/team8013/frc2024/controlboard/CustomXboxController.java). And one TBS Mambo Controller for     driving

- [com.team8013.frc2024.shuffleboard](https://github.com/maxconine/8013-2024-Crescendo-Imported-v2/tree/Public-Code-2024/src/main/java/com/team8013/frc2024/shuffleboard)

  Contains layouts for reporting telemetry to the Shuffleboard. Entries are organized into Tabs, which extend the ShuffleboardTabBase. Superstructure tab is neatly organized.

- [com.team8013.frc2024.subsystems](https://github.com/maxconine/8013-2024-Crescendo-Imported-v2/tree/Public-Code-2024/src/main/java/com/team8013/frc2024/subsystems)

  Contains code for all subsystems, with one singleton implementation per subsystem. Subsystems extend the Subsystem abstract class. Each subsystem's logic is contained in an enabled     loop, a read periodic inputs method, and a write periodic outputs method, which are called by the SubsystemManager class. Subsystems are called from Superstructure.java
