# Discussion Questions - Recommender Systems

## Big Picture Ideas

1. **Why do we need recommender systems AT ALL?**

- Short tail vs. Long tail
  - Can people come up with examples of each?
  - Another way to think about it: 
    - Big stores only have so much space, so limited to "big brands"
    - Digital stores can have infinite options
    - You could see "everything" in a box store in an hour, not possible with digital stores

- What is the motivation for the digital store?

  - Increase sales or engagement

- Is increasing sales or engagement *ethical*?

  

2. **What's the real world data to consider?**

- Users
  - Things they do (behavior)
  - Things they are (demographic)
- Products
  - Attributes of the product
- Different relationships to consider:
  - User with Product
    - Users like (or dislike) certain products
    - Users can give a rating (or preference) to different products
  - Product with Product
    - Products can be similar or different from each other
    - This similarity can be rated and ranked
  - User with User
    - Users can be similar or different from each other

3. **How do we get data on these users, products, or relationships?**

- Users can supply their own information explicitly
  - Fill out a form, survey, etc.
- Users can be monitored and information about them inferred
  - Can construct a "model" for the user
- Products are tagged manually, typically by the service provider
- Rating the relationships:
  - User-Product
    - Explicit ratings
    - Implicit ratings through interaction and usage
  - Product-Product
    - Can be computed from service provider data
  - User-User
    - Can be computed from user-generated data

4. **What are the different types of recommender systems?**

- Recommender Systems:
  - Content-based
    - All content or products must be properly characterized
    - Recommends similar products to the user
    - Pros:
      - Simple to use, can easily recommend new products without any knowledge of user
    - Cons:
      - Cannot find novel products
      - Must have all products characterized
      - Products cannot carry subjective information
  - Collaborative Filtering (user-user filtering)
    - Users are characterized by past purchases or interactions
    - Users can then be compared with OTHER users to find similarities
    - Recommends similar products that other similar users purchased
    - Thought idea: "like a friend recommending a product"
    - Pros:
      - Can find novel products
      - Offers a much richer recommendation
      - No need for products to have all information (or any!)
    - Cons:
      - Cold-Start, new users or products cannot be recommended
        - How do modern companies overcome this?
      - Heavily favors popular products
      - "Gray Sheep", or users with mixed preferences, are hard to recommend
  - More advanced
    - Construct a model for a user, so ratings on products can be predicted
    - Recommendations are based on the model, not specific users

5. **Ways to measure "similarity"?**

- First, all attributes for users and products must be quantified
- Similarity is then measured as the "distance" between users/products
  - How can there be different "distances" between the same two points?
- Several ways to measure distance:
  - Euclidean Distance
    - L2 Norm, Ruler Distance
  - Cosine Similarity
  - Pearson Coefficient
  - Jaccard Similarity
  - Hamming Distance
  - SVD

