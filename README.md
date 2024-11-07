N=500
p=100
Actual_positive = 50
TP = 45

FP = p-TP
FN = Actual_positive - TP
TN = N-(TP + FP +FN)

Accuracy = (TP + TN) / N
Precision = TP / (TP + FP)
Recall = TP / (TP + FN)

print("Confusion Matrix")
print(f"{TP}\t{FP}\n")
print(f"{FN}\t{TN}\n")

print("\n")
print("Metrics Final Answer: ")
print("Accuracy: ", Accuracy)
print("Precision: ",Precision)
print("Recall: ",Recall)
