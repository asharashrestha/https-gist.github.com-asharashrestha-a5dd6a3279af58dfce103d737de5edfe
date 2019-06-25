# Modification to Apriori Algorithm to allow only events which are consecutive. <br/>
For example, if we have the medical event as:
admission -> diagnosis -> treatment, then the rules produced by the algorithm cannot have the ordered altered. <br/>
Valid rules would be:<br/>
admission -> diagnosis<br/>
diagnosis -> treatment<br/>
admission, diagnosis -> treatment<br/>
admission -> diagnosis, treatment<br/>

# Invalid rules will be: <br/>
diagnosis -> admission<br/>
treatment -> admission<br/>
treatment -> diagnosis<br/>
treatment -> admission, diagnosis<br/>
treatment, diagnosis -> admission<br/>
diagnosis -> admission, treatment<br/>
