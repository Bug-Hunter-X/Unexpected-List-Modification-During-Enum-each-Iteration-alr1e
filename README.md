# Elixir List Modification Bug

This repository demonstrates an issue in Elixir involving unexpected list modification. When attempting to remove an element from a list within an `Enum.each` loop, the list remains unchanged because `Enum.each` does not mutate the list itself.

## Bug Description
The code iterates through a list and tries to delete an element if it matches a specific value. However, the modification performed within the loop does not affect the original list.

## Bug Solution
The solution involves using a different approach to list modification that does not mutate the list while iterating.