# Architecture Snapshot

## Goal

HydroAbyss is designed as a lean web platform for maritime authority building, specialised lead generation, and technical content delivery.

The product is intentionally simple in its runtime model:

- static-first public site
- lightweight interactive layer
- selective backend endpoints where business workflows require them

## High-level design

### Public content layer

The visible product is built around:

- landing/home experience
- service pages
- sector and case-oriented pages
- technical articles and long-form guides
- authority/profile pages

This keeps most of the site cache-friendly and operationally simple.

### Dynamic layer

A smaller backend surface supports:

- inquiry/contact capture
- internal review workflows
- selected business administration needs

This boundary is deliberate. It keeps the public site light while preserving operational capability.

## Main design choices

### 1. Static-first architecture

Reason:

- lower operational complexity
- easier performance control
- better SEO predictability
- easier editorial scaling for long-form content

### 2. Lightweight frontend

Reason:

- faster page delivery
- lower dependency footprint
- easier long-term maintenance
- strong fit for content-heavy, service-led pages

### 3. Backend only where it creates business value

Reason:

- avoid unnecessary application complexity
- keep admin and inquiry logic separate from the public surface
- reduce risk when publishing public artifacts

### 4. Structured service/content architecture

Reason:

- the platform is not only informational
- it needs to support authority, discovery, and conversion at the same time

## Areas intentionally excluded from the public showcase

- deployment automation
- internal admin flows
- operations documentation
- raw working assets
- private environment details
- business playbooks

## What the public repo should prove

- product judgment
- technical clarity
- architectural restraint
- ability to build real business-facing platforms

It does not need to expose every implementation detail to be useful in hiring or technical review.
