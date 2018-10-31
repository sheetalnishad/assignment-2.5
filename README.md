1. States = rownames(US Arrests)
Get states names with ‘w’.
Get states names with ‘W’.
Ans. USArrests
States = rownames(USArrests)
States

# Get states names with 'w'.
States[grep("w", States)]
#Get states names with 'W'.
States[grep("W", States)]



2. Prepare a Histogram of the number of characters in each US state.
Ans. df <- nchar(States)
df
hist(nchar(States))
States <- rownames(USArrests)
No_of_Char <- nchar(x)
df <- data.frame(States, No_of_Char)
df
barplot(df$No_of_Char, main = "Number of Characters in Each US State",
        xlab = "States", ylab = "No. of Character in Each State",
        col = "blue", axes = TRUE
)

