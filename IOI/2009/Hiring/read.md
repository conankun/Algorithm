<b>*** veritifed ***</b><hr>
Our purpose is to maximize people to hire(if same, minimize the cost)<br><br>

Let's suppose G the group of selected workers<br><br>

Then for worker i, his payment is Q<sub>i</sub> * (maximum cost per unit qualification level among the group members)<br>
(*unit qualification level means Q<sub>i</sub>=1<br> and cost per unit qualification is determined by S<sub>i</sub>/Q<sub>i</sub>)<br><br>

To solve this, sort according to S<sub>i</sub>/Q<sub>i</sub> and let's set maximum cost per unit qualification level among the group members S<sub>i</sub>/Q<sub>i</sub>(let's call it MC)<br><br>

Iterating from N to 1, remove(using max-heap) all employees from employeed list that appeared before i-th element and add(using min-heap) employees to employed list according to qualification level(ascending order) that appeared before i-th element(includes itself) until total cost exceed total Budget W. (Total cost is MC * sum of Qualification level in the employeed list) If you can employ more people or same people with less cost, replace the existing answer.<br><br>

It will take O(NlgN) time finally.
