# Netlix-Movie-Analysis

Hypothesis: The average duration of movies has declined over a period of time

# Set the figure style and initalize a new figure
plt.style.use('fivethirtyeight')
fig = plt.figure(figsize=(12,8))

# Create a scatter plot of duration versus release_year
#netflix_movies_col_subset.plot(x="release_year", y="duration", kind="scatter", c=colors)

plt.scatter(x="release_year", y="duration", data=netflix_movies_col_subset, c=colors)

# Create a title and axis labels
plt.title("Movie duration by year of release")
plt.xlabel("Release year")
plt.ylabel("Duration (min)")

# Show the plot
plt.show()



