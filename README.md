# Healthcare
sub=weight_kg,height_m,age,systolic,diastolic
subject=[80,1.6,70,120,80]
for sub in subject:
    print_results(weight_kg,height_m,age,systolic,diastolic)
print(subject1)
def bmi_calc(weight_kg,height_m):
    bmi=int(weight_kg/height_m**2)
    return bmi
def predict_max_HR(age):
    max_HR=220-age
    return max_HR
def bp_risk(systolic,diastolic):
    if systolic>=120 and systolic<130 and diastolic<80:
       bprisk="elevated BP"
    elif(systolic>=130 and systolic<140) or (diastolic>=80 and diastolic<90):
       bprisk="stage hypertension"
    elif systolic>=140 or diastolic>=90:
       bprisk="stage 2 hypertension"
    else:
       bprisk="invalid"
    return bprisk
def print_results(bmi,max_HR,bprisk):
    bmi=int(weight_kg/height_m**2)
    max_HR=220-age
    bprisk=bp_risk(systolic,diastolic)
print("\tweight_kg={}_kg".format(weight_kg))
print("\theight_m={}_m".format(height_m))
print("\tage={} years old".format(age))
print("\tblood prseeure ={}/{}".format(systolic,dystolic))
print("\tbmi={}".format(bmi))
print("\tmax_HR={} bpm".format(max_HR))
print("\tblood pressure= "+bprisk)
print("\n")
