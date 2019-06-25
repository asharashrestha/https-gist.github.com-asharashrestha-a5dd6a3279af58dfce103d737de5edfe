# Modification to Apriori Algorithm to allow only events which are consecutive. For example, is we have the medical event as:
## admission -> diagnosis -> treatment, then the rules produced by the algorithm cannot have the ordered altered. 
# Valid rules would be:
# admission -> diagnosis
# diagnosis -> treatment
# admission, diagnosis -> treatment
# admission -> diagnosis, treatment

# Invalid rules will be: 
# diagnosis -> admission
# treatment -> admission
# treatment -> diagnosis
# treatment -> admission, diagnosis
# treatment, diagnosis -> admission
# diagnosis -> admission, treatment
