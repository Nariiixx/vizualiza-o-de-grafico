<h2>Sobre o projeto</h2>
<h3>o projeto é um vizualização de gráfico onde eu coloquei em prática o que eu aprendi no cursinho sobre dados</h3>
<h3>tecnolgias usadas:</h3>
<ul>python 3.x</ul>
<ul>pandas</ul>
<ul>seaborn</ul>
<ul>matplotlib</ul>
<p></p>
<p>código final</p>
<p>plt.figure()
plt.subplot(1, 2, 1)
srn.histplot(data.PIB, kde=True, bins=10).set(title='PIB')

plt.subplot(1, 2, 2)
srn.histplot(data.VALOREMPENHO, kde=True, bins=10).set(title='valor empenho')


agrupado = data.sort_values('PIB').head(10)
agrupado = agrupado.iloc[:,1:3]
agrupado.plot.bar(x='MUNICIPIO', y='PIB', color='gray').set(title='10 municípios com  PIB')


agrupado = data.sort_values('VALOREMPENHO').head(10)
agrupado = agrupado.iloc[:,[1,3]]
agrupado.plot.bar(x='MUNICIPIO', y='VALOREMPENHO', color='gray').set(title='10 municípios com valor empenho')
</p>

