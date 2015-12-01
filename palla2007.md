# Quantifying social group evolution
*Palla, Barabasi, Vicsek*

* We have developed an algorithm based on clique percolation that allows us to investigate the time dependance of overlapping communities on a large scale, thus uncovering basic relationships characterizing community evolution.
* networks capturing collaboration between scientists and calls between mobilde phone users
* **large groups** persist longer if they are capable of dynamically altering their membership
* **small group** condition for stability is that their composition remains unchanged
* knowledge about time commitment of members can estimate lifetime of community
* dynamics of small and large groups

## Data
* 142 month, monthly list of publications, 30.000 authors
* 52 weeks of phone calls of one mobile phone company, 4 milion users
* collaboration event: phone call or publication

## Network Characteristics (local structure)
* co-authorship: dense network, overlap between communities is very significant, long term collaboration process
* cell-phone: less interconected, seperated by inter-community nodes/edges, instant communication
* phone call between two people, authors can be more than two (fully connected clique)
* co-authors: long term collaboration process
* phone-call: instant communication

## Extracted Communities and their parameters
* communities were extracted using the clique percolation method
* first step: check if uncovered communities correspond to groups of individuals with a shared common activity pattern
* compared average weight of links inside communiy to average weight of inter-community links
* found out that collaboration/communication within groups is inside community higher

## Community Events and matching
* community can grow or contract, groups may merge or split, communitites are born or disappear
* developed method for matching subsequent states of evolving communities for relatively distant points in time

## Definitions: size, age, auto-correlation, stationarity
* basic quantities for characterizing a community: **size** ´s´, **age* ´T´ (time passed since birth)
* `s` and `T` are positivley correlated: larger communities are on average older
* auto-correlation function, to quantify the overlap between to states of the same community `A(t)` at `t` timesteps apart
* collaboration networks are more *dynamic*
* decays faster for larger communities (membership of larger communities is changing at a high rate
* in contrast smaller communities change at smaller rate (composition more or less static)
* define average correlation between subsequent states (**stationarity**) for a community

## Headline
* 
