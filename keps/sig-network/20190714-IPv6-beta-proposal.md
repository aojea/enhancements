---
title: graduate-ipv6-to-beta
authors:
  - "@aojea"
owning-sig: sig-network
participating-sigs:
reviewers:
  - "@bentheelder"
approvers:
  - "@lachie83"
  - "@thockin"
editor: TBD
creation-date: 2019-07-14
last-updated: 2019-07-14
status: implementable
see-also:
replaces:
superseded-by:
---

# Graduate IPv6 Support to beta

## Table of Contents

<!-- toc -->
- [Summary](#summary)
- [Motivation](#motivation)
  - [Goals](#goals)
- [Proposal](#proposal)
  - [User Stories](#user-stories)
- [Design](#design)
  - [Test Plan](#test-plan)
    - [Needed Tests](#needed-tests)
  - [Graduation Criteria](#graduation-criteria)
- [Implementation History](#implementation-history)
<!-- /toc -->

## Summary



## Motivation

Kubernetes have IPv6 support as Alpha feature since v1.9. Since then, the code and API has been stabilized and CI testing was implemented. Therefore, we would like to graduate IPv6 support from Alpha to Beta.

### Goals

* Promote IPv6 support to beta version.

## Proposal

### User Stories

* A user can deploy, operate and use a kubernetes cluster in an IPv6 only environment. 

## Design

### Test Plan

#### Needed Tests

- Run a CI with conformance E2E tests on an IPv6 only kubernetes cluster.

### Graduation Criteria
- [ ] Have IPv4 feature parity
- [x] Have E2E test
- [x] Is documented

## Implementation History

- [IPv6 Support was introduced as alpha in kubernetes 1.9](https://github.com/kubernetes/kubernetes/blob/master/CHANGELOG-1.9.md)
- [IPv6 Support enhancement request](https://github.com/kubernetes/enhancements/issues/508)
- [IPv6 implementation tracking issue](https://github.com/kubernetes/kubernetes/issues/1443)
- [IPv6 CI](https://testgrid.k8s.io/conformance-kind#kind%20(IPv6),%20master%20(dev)) 
- [Kind IPv6 support](https://github.com/kubernetes-sigs/kind/pull/636)
