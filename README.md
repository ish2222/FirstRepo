# FirstRepo

with Result as
(select Salary,Dence_Reank() over (order by salary desc) as DenceRank from Employee)
select salary from Result where Result.DenceRank=2
