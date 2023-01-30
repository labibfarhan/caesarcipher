def encrypt (text,n):
	result = ""
	for i in range (len(text)):
		char = text[i]
		result += chr ((ord(char) + n - 65) % 26 + 65)
	return result
	


text = "ICEDEPARTMENTDIU"
n = 4
print (encrypt (text,n)) 