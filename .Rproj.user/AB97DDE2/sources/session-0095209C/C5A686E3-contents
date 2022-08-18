#---- Practicing Reprex #---

# Not A Reprex
library(tidyverse)
library(palmerpenguins)

penguins |> 
  select(species, body_mass_g, flipper_length_mm, year) |> 
  filter(species == "Chinstrap") |> 
  str_to_lower(species) |> 
  group_by(island) |> 
  summarize(mean(body_mass_g, na.rm = TRUE),
            mean(flipper_length_mm, na.rm = TRUE))

### A REPREX
library(tidyverse)

warpbreaks |> 
  str_to_lower(wool)

### A Fixing Reprex
library(tidyverse)

warpbreaks |> 
  mutate(wool = str_to_lower(wool))


### REPREX WITH A SYNTHESIZED DATA FRAME
library(tidyverse)

upper_case <- tribble(
  ~letter,
  'A',
  'B',
  'C'
)

upper_case |> 
  str_to_lower(letter)
