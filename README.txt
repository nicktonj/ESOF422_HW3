Andrew Dixon and Nicolas Tonjum

Tips and Tricks for our game:
- Player starts out at level 1.
- Health increases and decreases based on level.
- Defeating an Opponent increases player's level, therefore their health.
- After defeating an Opponent, player's health is reset to max health.
- Dying to an Opponent decreases player's level.
- Going below level 1 results in death state, which means player must reset entire game.
- Running from Opponent results in players and opponents health reseting to max health.
- There are 3 Opponents, Opponent1, Opponent2, Opponent3.
- Each Opponent is a different level: levels 1,2, and 3.
- There are 5 functions
	- see_opponent(o:Opponent)
	- attack(i:Integer)
	- receive_blow(i:Integer)
	- run_from_opponent()
	- reset()

The necessary code to get this going is:

!create f1:FPS
!f1.initInstance()
!insert (Neutral1,f1) into firstPersonShooterState
!insert (Die1,f1) into firstPersonShooterState                                
!insert (Panic1,f1) into firstPersonShooterState
!insert (Attack1,f1) into firstPersonShooterState
!insert (Opponent1, f1) into opponentFight
!insert (Opponent2, f1) into opponentFight
!insert (Opponent3, f1) into opponentFight


After running above code, you can run below code line by line or run anything else you want:

!f1.see_opponent(Opponent1)
!f1.attack(25)
!f1.receive_blow(99)
!f1.attack(75)
!f1.see_opponent(Opponent3)
!f1.attack(75)
!f1.receive_blow(115)
!f1.run_from_opponent()
!f1.see_opponent(Opponent2)
!f1.attack(75)
!f1.receive_blow(100)
!f1.attack(50)
!f1.receive_blow(100)
!f1.see_opponent(Opponent1)
!f1.attack(100)
!f1.see_opponent(Opponent2)
!f1.attack(200)
!f1.see_opponent(Opponent3)
!f1.attack(300)
!f1.see_opponent(Opponent3)
!f1.receive_blow(400)
!f1.see_opponent(Opponent3)
!f1.receive_blow(300)
!f1.see_opponent(Opponent3)
!f1.receive_blow(200)
!f1.see_opponent(Opponent1)
!f1.receive_blow(100)

