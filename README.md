# tr_cohort_job_matching-
Function clear monitor
  Pass In: nothing
  Direct the operating system to clear the monitor
  Pass Out: nothing
Endfunction 

Function match individual A characteristics with job A characteristics
  Pass In:  “wants to work remote” “react experience” “looking for frontend” "flexible working hours"
  If it matches exactly Job characteristics A “remote” “flexible working hours” "react" "frontend developer" then score 100
  Pass Out: display "Matched with jobs" and produce matching jobs
Endfunction 

Function non match individual A characteristics with job A characteristics
  Pass In: nothing or non matching characteristics
  Call: clear monitor
  Pass Out: value zero to the operating system and display 0 matching jobs
Endfunction

Function match individual B characteristics with job B characteristics
  Pass In:  “remote” “react experience” “looking for frontend” "flexible working hours"
  If it matches exactly Job characteristics A “remote” “flexible working hours” "react" "frontend developer" then score 100
  Pass Out: display "Matched with jobs" and produce matching jobs
Endfunction 

Function non match individual B characteristics with job B characteristics
  Pass In: nothing or non matching characteristics
  Call: clear monitor
  Pass Out: value zero to the operating system and display 0 matching jobs
Endfunction

Function generate score between 0 and a 100 depending on match
