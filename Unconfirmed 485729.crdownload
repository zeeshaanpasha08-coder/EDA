import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

df = pd.read_excel("titanic.xlsx")

print(df.head())
print(df.info())
print(df.describe())
print(df.isnull().sum())

df.hist(figsize=(10, 6))
plt.show()

plt.figure(figsize=(10, 6))
sns.boxplot(data=df)
plt.show()

plt.figure(figsize=(8, 5))
sns.heatmap(df.select_dtypes(include='number').corr(), annot=True, cmap="coolwarm")
plt.show()

sns.pairplot(df)
plt.show()
