---
title: Troubleshoot the OperationPreempted error code
description: Learn how to troubleshoot the OperationPreempted error when you try to create and deploy an Azure Kubernetes Service (AKS) cluster.
ms.date: 3/10/2022
author: DennisLee-DennisLee
ms.author: v-dele
editor: v-jsitser
ms.reviewer: rissing, chiragpa, erbookbi
ms.service: container-service
#Customer intent: As an Azure Kubernetes user, I want to troubleshoot the OperationPreempted error code so that I can successfully create and deploy an Azure Kubernetes Service (AKS) cluster.
---
# Troubleshoot the OperationPreempted error code

This article describes how to identify and resolve the `OperationPreempted` error, which might occur if you try to create and deploy a Microsoft Azure Kubernetes Service (AKS) cluster.

## Symptoms

When you try to deploy the cluster, you receive the following error message:

> This operation has been preempted by Deleting operation.

## Cause

In most cases, this error occurs when an in-progress create operation was interrupted by a subsequent delete operation that was issued before the create cluster operation has completed.

## Solution

Retry the operation after the delete operation is completed.

## More information

- [General troubleshooting of AKS cluster creation issues](troubleshoot-aks-cluster-creation-issues.md)
