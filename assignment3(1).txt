% reverse the empty list
reverse([], []).

% reverse a list of one element
reverse[[X], [X]).

% if there is more than 1 element in the list
reverse([X|Xs], R):-

  % reverse the tail and append the head to the new tail
  reverse(Xs,T), append(T, [X], R ).