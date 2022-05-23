# Cheap DAO

## Inspiration
Currently there are mainly two ways for building a DAO. Either creating a completely on-chain DAO or creating a semi on chain DAO using a multisig wallet. The disadvantage of the first option is the high gas price of ethereum network, due to which not everyone can vote and the disadvantage of the second option being less decentralisation. 

## What it does
CheapDAO is a set of smart contracts using which one can deploy the treasury contract on the ethereum network and the governance contract on the polygon chain, so users can vote on the polygon network utilising the cheap gas fee of the polygon pos chain, then the actions are executed on the ethereum network.

## How I built it
I utilised the polygon state transfer mechanism to trigger the execute proposal function on the treasury contract(which is on ethereum network) from the governance contract(which is on polygon network) if the proposal is passed by majority votes. 

## Challenges I ran into
Finding a solution for the DAO high gas fee problem was not easy, and took a lot of time. And also how to structure both the contracts took some time.

## Accomplishments that I'm proud of
Using this system, the DAO token holder irrespective of their holding size will be able to vote without worrying about the high gas fees, thus resulting in a more fare voting process.

## What I learned
I have learned about the cross chain communication between polygon pos chain and the ethereum chain, and also the DAO structures.

## What's next for CheapDAO
I am planing to add a second treasury on the polygon network also, so users will be able to vote for actions on both the networks (ethereum and polygon networks).
