# Regex
How to use the regular expression.

genesys = re.compile(r'Abuja', re.I)
genesys = genesys.sub('Lagos','Abuja is a place to be.I have money in abuja in Nigeria. ')
print (genesys)

agent = re.compile(r'Agent (\w\w)\w*')
agent = agent.sub(r'\1****','Agent James told Agent Carol that Agent Eve knew that Agent Bond is double Agent.')
print (agent)


card = re.compile(r'((\d){4})(\w){8}\w*((\d){4})')
card = card.sub(r'\1********\4','0000999977776666')
print (card)
