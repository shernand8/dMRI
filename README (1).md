# What we learned
## Week one 
Throughout the week, we began to have daily meeting at [Saint Justine's](https://www.chusj.org/). 

We started to learn how to code with python. We began by creating two simple graphs which plotted the distributions of birth age and birth weight of a sample of 90 babies. Here are some highlights. 

	plt.figure(figsize=(5,5))

	plt.hist(scan_age,color='r',bins = 18)

	plt.title('Birth Weight Distribution')

	plt.xlabel('Birth Weight (in kg)')

	plt.ylabel('Frequency')

Next we learned how to create a bar graph that would plot different categories along the same axis. We also displayed a legend for the first time and learned how to include error bars. Here are some highlights. 

	plt.bar([9, 10, 11],Height_bar3, width = 0.5, color = ['red', 'orange', 'blue'])

	plt.errorbar([9, 10, 11], [ave_shc_vpreterm, ave_shc_modpreterm, ave_shc_term], yerr = [np.std(vpreterm1 ['scan_head_circumference'].values), np.std(modpreterm1 ['scan_head_circumference'].values), np.std(term1 ['scan_head_circumference'].values)], fmt = 'o', color = 'black', markersize = 2)

Our next challenge was to graph a scatter plot, this time using data from all the babies that we had access to. We also had to include a trendline. Here are some highlights. 

	a, b = np.polyfit(df['birth_age'].values, df['birth_weight'].values, 1)

	plt.plot(df['birth_age'].values, a*df['birth_age'].values+b, color = 'black')

## Week two
We learned MRI safety. Here are some important things to consider. 

 - Ferromagnetic objects should not be brought into the MRI room
 - Other metallic objects should not be worn while being scanned because they can heat up quickly and cause burns 
 - Certain medical implants should not be brought into the MRI room because they will cease to function
 - The MRI machine should only be quenched in emergency scenarios because it is a very expensive process

> Written with [StackEdit](https://stackedit.io/).

