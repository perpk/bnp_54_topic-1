## ---------------------------
##
## Script name: Main.R
##
## Purpose of script: 
##  Solutions to the 1st exercise of the 1st Assignemt for the BNP54 class
##
## Author: Konstantinos Perperidis
##
## Date Created: 2024-03-23
##
## Email: k.a.perperidis@gmail.com
##        std531050@ac.eap.gr
##
## ---------------------------

library("stringi");

source("GetOccurenceCount.R");
source("GetOccurencePositions.R");

# Init
set.seed(1);
data <- stringi::stri_rand_strings(1, 2000, '[ACGT]');

# Vectorization of character sequence
dataAsVector <- strsplit(data, NULL)[[1]];

# Part 1 - Count of occurence absolute and percentual
dataFactor <- factor(dataAsVector, c('A', 'C', 'G', 'T'));
dataTable <- table(dataFactor);
dataPropTable <- prop.table(dataTable);

# Part 2 - Call a function to return the count of a given character in the sequence
getOccurenceCount('A', data);

# Part 3 - Call a function to return a list with the positions within the sequence
getOccurencePositions('A', data);
