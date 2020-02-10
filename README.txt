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

!f1.see_opponent(Opponent1)
!f1.attack(50)
!f1.receive_blow(99)
!f1.attack(50)