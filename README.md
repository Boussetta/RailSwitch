# RailSwitch

The system dynamics is relative to the diagram given by the figure bellow. It’s about two trains 
”Tr1” and ”Tr2” which are
following, at different speeds, two rails located in a zone divided into four sub areas. The two 
lanes are connected using a switch system operating as following: When a train, moving on a lane, 
reaches a switch which was already activated (actions ”S1” or ”S2”), it heads toward the other 
lane. Initially, the two switches are disabled. The train ”Tr1” can make round trips between ”A1” 
and ”C1”. The train ”Tr2” can make round trips between ”A2” and ”C1” or ”C2” with respect to the 
following specifications:

• Initially: the two switches are disabled, ”Tr1” and ”Tr2” are respectively in ”A1” and ”A2”. When 
pushing on the button ”M” the two trains starts to advance (actions ”Ad1” and ”Ad2”).

• When ”Tr1” arrives to ”B1”: if ”Tr2” is in the ”zone 4” then ”Tr1” stops until ”Tr2” exits the 
”zone 4”. Then ”Tr1” resumes, and when it reaches ”C1” the train goes back to ”A1” (action ”Ba1”) 
where it stops.

• When ”Tr2” arrives to ”B2”, we are confronted to two cases: 
    First case: if ”Tr1” is already in ”zone 2” then ”Tr2” continues its advance toward ”C2” and then returns to ”A2”. 
    Second case: if ”Tr1” is not yet in ”zone 2” then ”Tr2” then ”switch 2” is enabled (S2=1) and ”Tr2” advances toward 
    ”C1”. When ”Tr2” reaches ”C1”, ”switch 2” is disabled (S2=0) and ”switch 1” is enabled (S1=1). Then 
    ”Tr2” go back to ”A2” in where it stops. ”switch 1” is disabled when ”Tr2” exits the ”zone 4”.

•  ”Tr1” is prior in the case where the two trains reaches ”B1” and ”B2” at the same time.
