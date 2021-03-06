CS537-P4
========

Project 4 from CS 537 at University of Wisconsin-Madison taught by Laura 'Hobbes' Legault

Program 4: Multithreaded Web Server with Statistics

Programmers: Peter Collins (pcollins) and Brennan Schmidt (bschmidt)

This program is multithreaded web server that returns statistics of the requests in the response header.  It has several parameters it can take in including: the port number it runs on, the number of threads it uses, the number of requests it allows at a time, and the scheduling algorithm/policy that it uses to process priority of requests.  The policies are first-in, first-out (FIFO), smallest file first (SFF), and smallest file first with bounded starvation (SFF-BS).  Each is progressively more complex, but with faster response times. For FIFO we used a standard queue based on an array. For SFF we used a priority queue based on a sorted array sorted with quick sort.  For SFF-BS we used a queue array of priority queues based on an array and the implementation in SFF.

