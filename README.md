
The below command will help list the constituents of any package in R

```{r}
ls("package:dplyr")
```

--------------------------------------------------------------------

The ggtheme assist is helpful in customising the ggplot charts using a UI

```{r}
# ggplot addin 
install.packages("ggThemeAssist")


# character manipulation in dplyr
diamonds %>% group_by(color) %>% summarize(cuts=paste(unique(cut), collapse=","))

# Select the Addin and do the manual customisation using ggtheme dropdown
```

--------------------------------------------------------------------
the `cut()` function in R helps to discretize a continous variable

```{r}
ggplot(data = ncbirths, 
       aes(x = weeeks, y = weight)) + 
  geom_boxplot()
```

`vs`

```{r}
ggplot(data = ncbirths, 
       aes(x = cut(weeks, breaks = 6), y = weight)) + 
  geom_boxplot()
```
-------------------------------------------------------------

`ggplot2` provides several different mechanisms for viewing transformed relationships. The `coord_trans()` function transforms the coordinates of the plot. Alternatively, the `scale_x_log10()` and `scale_y_log10()` functions perform a `base-10` log transformation of each axis. 

-------------------------------------------------------------

`skimr` package in r is a useful way of doing the EDA in R. 

Use the `skim` function from `skimr`. 
`skim(data)`

This can also be used post grouping a variable

```{r}
data %>%
 group_by(v1) %>%
  skim()
```  
  




