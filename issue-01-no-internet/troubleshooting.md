# Issue 1: No Internet Connectivity

## Problem

The computer cannot access the internet.
Websites fail to load and network connectivity appears limited.

## Initial Observation

The network icon showed that the device was connected to WiFi but websites were not loading.

## Step 1: Check IP Configuration

Open Command Prompt and run:

ipconfig

This command displays the IP address assigned to the computer.

## Step 2: Test Local Network Connectivity

ping 192.168.1.1

This tests whether the computer can communicate with the router.

## Step 3: Test Internet Connectivity

ping google.com

If this fails, the problem may be DNS related.

## Step 4: Flush DNS Cache

ipconfig /flushdns

## Solution

The issue was caused by a DNS resolution problem.
Flushing the DNS cache restored internet connectivity.

## Commands Used

ipconfig  
ping  
ipconfig /flushdns
