# Introduction to Transformers

## Overview
This repository contains content derived from a research paper providing a detailed introduction to transformers in machine learning. Transformers are neural network components that have significantly advanced various domains such as natural language processing, computer vision, and spatio-temporal modeling. While there are many resources available on transformers, they often lack precise mathematical descriptions and clear explanations of design choices. This README serves as a guide to understanding the content provided in this repository.

## Objective

The primary goal of this repository is to offer a mathematically precise and intuitive understanding of transformer architecture. It aims to fill the gap in existing literature by providing clear explanations of transformer components and design choices.


## Target Audience

This resource is intended for researchers, practitioners, and students with a solid understanding of machine learning fundamentals who seek a deeper understanding of transformers.


## 1. Preliminaries
- In this section, we'll discuss the format of the input data for a transformer, the transformer's objective, and the format of its output.

### 1.1 Input Data Format: Sets or Sequences of Tokens
In order to apply a transformer, data must be converted into a set or sequence of N tokens x(0) n of dimension D (see figure 1). 
The tokens can be collected into a matrix X(0) which is D × N.

- To grasp how transformers work, let's consider real-world examples of input data:

1. Text Input:

- Imagine you have a paragraph of text. To feed it into a transformer, you break it down into a sequence of words or sub-words. Each word is then represented by a unique vector.

- For instance, the sentence "The cat sat on the mat" could be tokenized into individual words: ["The", "cat", "sat", "on", "the", "mat"].

2. Image Input:

- Now, picture an image. To feed it into a transformer, we divide the image into smaller chunks called patches. Each patch gets turned into a vector.

- For example, if we're looking at a photo of a dog, we might divide it into different parts like the dog's face, tail, or body.

**Now, there are two ways we can handle these representations:**

## **Fixed Embeddings**: 

We keep the vector representations of words or image patches the same throughout the process.

- **Text Example**:
	
	Imagine we're looking at movie reviews to see if they're positive or negative. We assign each word in a review a fixed way of being represented, like a label. So, the word "good" always gets the same label, no matter where it shows up or what movie it's talking about.

**Image Example:**

  Let's say we're sorting pictures of animals. Each little part of a picture, like a spot of fur or a bit of an animal's face, gets a fixed way of being represented, like a tag. So, a part representing a dog's tail always gets the same tag, no matter what kind of dog it is or where the tail is in the picture.

- **Learned Embeddings** : we can tweak these vector representations while the model is learning, to make them better suited for the task at hand.





