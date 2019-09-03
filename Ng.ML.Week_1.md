# UnSupervised Learning ➟ ➡ ⤇ ⇛

## Clustering

## Cocktail Party Problem - Algorithm

- separates out the data from a MIX

> Octave - would be used to implement prototypes
>
> Octave - Prototyping tool

## Model Representation

- `supervised learning` - given the `right answer` for the each example in the test-data
  - `Regression Problem` - predicting the real-valued output
  - `classification Problem` - we are looking for discrete valued output
- Data set to train on is called  ***Training Set***
- Notations:
  - _`m` = number of input variables_
  - _`x`'s = "input" variables features_
  - _`y`'s = "output" variable / `target` variable_
  - ***`(x,y)` - training example***
  - ***`(xˆ(i), yˆ(i))` is `i`th training example***
- **flow:: `Training Set` ➡ `Learning Algorithm - LA`{JOB of the LA to give H} ➡ `{x}` ↠ `HYPOTHESIS - H` ↠ `{y}`**
  - **_`H`<sub>`𝛳`</sub>`(x)` = `𝛳` <sub>`0`</sub> + `𝛳`<sub>`1`</sub>`x`_** | _called Linear Regression with one Variable_
  - ***`y =` `H`<sub>`𝛳`</sub>`(x)`*** | _univariate linear regression_

## Cost Function

- ***`H`<sub>`𝛳`</sub>`(x)` = `𝛳` <sub>`0`</sub> + `𝛳`<sub>`1`</sub>`x`***
  - _`𝛳` <sub>`j`</sub> - Parameters_
  - **_How to choose `𝛳` <sub>`j`</sub>?_**
  - _By choosing different values of `𝜃`<sub>`j`</sub>, we get different `Hypothesis` functions_
  - _In a Linear Regression - We have a training set and have to find values of `𝜃`<sub>`0`</sub> & `𝜃`<sub>`1`</sub> so that we get a `straight line` which fits the DATA well_
    - _IDEA:: choose `𝜃`<sub>`0`</sub> & `𝜃`<sub>`1`</sub> so that `H`<sub>`𝜃`</sub> is close to `y` for our training examples `(x,y)`_
    - _minimize values of `𝜃`<sub>`0`</sub> & `𝜃`<sub>`1`</sub>_
    - `minimize` ***`1/2m`(`∑`<sub>`1`</sub><sup>`m`</sup>(`H`<sub>`𝜃`</sub>(`x`)<sup>`(i)`</sup> - `y`<sup>`(i)`</sup>)<sup>`2`</sup>***
      - _`m` is the number of training examples_
      - _`H`<sub>`𝛳`</sub>`(x)` = `𝛳` <sub>`0`</sub> + `𝛳`<sub>`1`</sub>`x`_

> Cost Function: minimize **`J(𝜃`<sub>`0`</sub>, `𝜃`<sub>`1`</sub>`)`** `=` ***`1/2m`(`∑`<sub>`1`</sub><sup>`m`</sup>(`H`<sub>`𝜃`</sub>(`x`)<sup>`(i)`</sup> - `y`<sup>`(i)`</sup>)<sup>`2`</sup>***
>
> Also called the `Squared Error Function`
