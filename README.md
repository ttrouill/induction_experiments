# Relation properties and families data sets

This repository contains the data for the experiments used in the paper:
*On Inductive Abilities of Latent Factor Models for Relational Learning*,
Théo Trouillon, Éric Gaussier, Christopher R. Dance, Guillaume Bouchard.


## Relation properties data

In the folder `relation_properties` are the generated matrices for each 
of the 13 combination of interest between reflexivity, symmetry and transitivity,
as described in the paper.
Matrices are saved in the `.mat` format under the variable name `y`.
They can be loaded from matlab or from python with the [scipy.io.loadmat](https://docs.scipy.org/doc/scipy/reference/generated/scipy.io.loadmat.html) function.
Ones represent positive samples, -1 negatives, and 0 missings (used for diagonal in
the non-[ir-]reflexive cases).

## Families data

The families data is represented in text files in the folder `families`, 
following a binary predicate syntax: *[!]relation(subject_entity,object_entity)*.
Leading `!` indicates a negative fact. Families are numbered from 1 to 5,
and the set of facts of each family is split between the four main relations
(father, mother, daughter, son) in files suffixed by `_4main.db`,
and the 13 other relations in files suffixed by `_13other.db`,
as described in the paper.


