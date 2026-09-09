# Baummethoden Frontend — Auto MPG Prediction UI

A Next.js (TypeScript) frontend that collects a car's specs and sends them to a prediction API to estimate fuel efficiency, built on top of a decision-tree model trained on the classic **Auto MPG dataset**.

## Screenshot

![Prediction form with sample input](/screenshot.png)

## What it does

The form collects the five features the model was trained on:

- **zylinder** — number of cylinders
- **ps** — horsepower
- **gewicht** — weight
- **beschleunigung** — acceleration
- **baujahr** — model year

On submit, the values are sent to a prediction API (configured via the `NEXT_PUBLIC_PREDICTION_API` environment variable) that serves the trained model and returns a predicted miles-per-gallon value.

## Status

The original backend prediction API was a temporary endpoint set up for a training course and is no longer active, so the live demo currently won't return a prediction result. The frontend itself is fully functional — see the screenshot above for the form working with sample input.

## Related project

This frontend was built to serve predictions from a decision-tree/random-forest model trained on the Auto MPG dataset (companion model-training project).

## Tech stack

`Next.js` · `TypeScript` · `React`
