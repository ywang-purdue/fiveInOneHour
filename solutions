from operator import itemgetter
# problem 1
def sumFromList(list):
	sum=0
	for i in list:
		if isinstance(i,str):
			i = float(i)
		sum = sum+i
	print sum

# problem 2
def appendToList(list, word1, word2):

	if word1 is None:
		pass
	else:
		list.append(word1)
	if word2 is None:
		pass
	else:
		list.append(word2)
	return list


def interweaveList(list1, list2):

	fulllist=[]
	maxlen=max(len(list1),len(list2))
	i=0
	while i < maxlen:
		try:
			fulllist = appendToList(fulllist, list1[i],list2[i])
		except:
			try:
				fulllist.append(list1[i])
			except:
				fulllist.append(list2[i])
		i = i+1
	return fulllist

# problem 3
def fibonacciNum(n):
	if n>2:
		return fibonacciNum(n-2)+fibonacciNum(n-1) 
	elif n==2:
		return 1
	else:
		return 0

def fibonacciSum(n):
	sum = 0
	for i in range(1,n+1):
		sum = sum + fibonacciNum(i)
	print(sum)

# problem 4

def largestCombo(list):
	newlist=[]
	maxlen = len(str(max(list)))
	for i in list:
		newlist.append(i*10**(maxlen-len(str(i))))
	indexlist = [i[0] for i in sorted(enumerate(newlist), key=lambda x:x[1])]
	ziplist = zip(indexlist,list)
	sortedlist = sorted(ziplist,key=itemgetter(0))
	sum = 0
	lenbefore=0
	for index,j in sortedlist:
		
		sum = sum+j*10**lenbefore
		lenbefore = lenbefore+len(str(j))
	print sum

# problem 5

def find100():
	baseline=['','1','','2','','3','','4','','5','','6','','7','','8','','9','==100']
	signs =['','+','-']
	equation=baseline
	for i in signs:
		equation[0] = i
		for i in signs:
			equation[2] = i
			for i in signs:
				equation[4] = i
				for i in signs:
					equation[6] = i
					for i in signs:
						equation[8] = i
						for i in signs:
							equation[10] = i
							for i in signs:
								equation[12] = i
								for i in signs:
									equation[14] = i
									for i in signs:
										equation[16] = i
										equString=''.join(equation)
										if eval(equString):
											print equString if eval(equString) else None



	
	



