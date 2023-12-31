# Wishing Tree
![image](https://github.com/0xambr0sia/wishing-tree/assets/147129231/ef25ac50-3ce6-4213-86f0-799c716afbac)

An interactive web experience that combines visual art, poetic messages, and dynamic animations to create a virtual "wishing tree." Users can click on the tree to reveal heartfelt wishes expressed in a visually captivating manner.

## Features
**Dynamic Animation:** The background image and wishes fade in and out gracefully with smooth animations.

**Text Scramble Effect:** Wishes are presented using a captivating text scramble effect, adding a touch of whimsy.

**Colorful Sparkle:** Each wish is adorned with a colorful sparkle, creating a visually engaging display.

**Randomized Transitions:** Transition phrases and edges are randomly selected for a diverse and unique user experience.

**Multilingual Support:** Wishes are available in multiple languages, reflecting the global nature of the community.

**Contributions:** Each wish is associated with a unique identifier, making it a collaborative and evolving art project.

## How to Use

Click anywhere on the page to toggle between the visual representation of the wishing tree and the poetic wishes. The background image fades out while the wishes fade in, accompanied by the mesmerizing text scramble effect and colorful sparkles.

## Contributors and Wishes

**ambr0sia.eth:** The wishing tree grows to encapsulate the soul of crypto culture. May it shine with our compassion, thirst for progress, and belief in collective hope.

**boredyachtapeclub.eth:** For love to speak first. I wish for peace to come over us all, soothing our souls.

**swallja.eth:** Certainty abandoned, forgiveness ordained. Apologies to ourselves, saying, "F**k it," and eating a hotpocket.

... and many more heartfelt wishes from the community!

## Inspiration
Inspired by the idea of a collective wishing tree in Japan as well as Yoko Ono's site specific wishing trees from the 1960s, this project aims to interrogate the notion of websites as new spaces for gathering, as well as to bring together diverse thoughts, hopes, and dreams into a visually stunning and interactive digital art piece.


This Solidity smart contract is named "wishingtree" and is designed to facilitate a decentralized wishing tree. Here's a description of the code:

## Contract Description
The contract is written in Solidity version 0.8.0 and includes OpenZeppelin and ManifoldXYZ libraries. It implements the Ownable contract, allowing the contract owner to have special privileges.

1. **Purpose**: The contract allows users to make wishes by invoking the `makeWish` function, which captures and stores their desires.

2. **Extension of Creator Core and TokenURI Interface**: This contract extends the `ICreatorExtensionTokenURI` interface from the ManifoldXYZ library. It also implements the `IERC165` interface.

3. **Events**:
   - `WishMade`: Fired whenever a wish is made. It includes the wisher's address, the wish text, and an acknowledgment message.

4. **State Variables**:
   - `baseTokenURI`: A string representing the base URI for token metadata.
   - `wishes`: An array of strings to store the wishes made by users.

5. **Modifiers**:
   - `onlyOwner`: Ensures that only the contract owner can execute certain functions.

6. **Functions**:
   - `supportsInterface`: Checks whether the contract supports a given interface.
   - `setBaseTokenURI`: Allows the owner to set the base token URI.
   - `mint`: Allows the owner to mint a new token with a specified extension URI.
   - `makeWish`: Allows users to make a wish. The wish is limited to 256 characters.
   - `tokenURI`: Retrieves the token URI for a given token ID.
   - `seeWishes`: Allows anyone to view the array of wishes made.

### Workflow
1. Users invoke the `makeWish` function to submit their wishes, which are then added to the `wishes` array.
2. The owner can set the `baseTokenURI` and mint new tokens with the `mint` function, which extends the Creator Core contract.

### Token URI
The `tokenURI` function is designed to return a base URI. In a complete implementation, this URI would be combined with the specific token ID to form the complete URI for the token's metadata.

### Note
Ensure that the required dependencies (OpenZeppelin and ManifoldXYZ) are properly installed when deploying this contract. Additionally, a complete implementation should include proper error handling and additional security considerations.

## License
This project is licensed under the [MIT License](https://chat.openai.com/c/LICENSE.md) - see the [LICENSE.md](https://chat.openai.com/c/LICENSE.md) file for details.

This project was created by ambr0sia. Feel free to connect with me on X at twitter.com/ambr0sia_xyz.
