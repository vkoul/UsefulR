
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

