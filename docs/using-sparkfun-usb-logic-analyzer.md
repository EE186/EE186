---
layout: default
title: Using the Sparkfun USB Logic Analyzer
description: Guide to capturing and analyzing digital signals with the Sparkfun USB Logic Analyzer.
nav_exclude: true
---

# Using the Sparkfun USB Logic Analyzer

A logic analyzer lets you observe multiple digital signals over time so you can debug protocols like I2C, SPI, and UART. We will use the SparkFun 8‑channel, 24 MHz USB Logic Analyzer (see product page: [SparkFun USB Logic Analyzer](https://www.sparkfun.com/usb-logic-analyzer-24mhz-8-channel.html)).

## What you need

- SparkFun USB Logic Analyzer and probe cable
- Your target board/circuit
- A computer with PulseView (Sigrok) installed

## Usage

PulseView is an open-source GUI for the Sigrok logic analysis stack. Install the correct version [here](https://sigrok.org/wiki/Downloads).

**Important Note:** For computers with Apple silicon, please download [PulseView 0.4.2](../assets/labs/PulseView-0.4.2.dmg).

Read [this](https://learn.sparkfun.com/tutorials/using-the-usb-logic-analyzer-with-sigrok-pulseview) guide to set up PulseView for the logic analyzer.

## Tips

- Connect the analyzer ground to your circuit ground. This is mandatory.
- Choose channels D0–D7 for the signals you want to observe.
- Optional: set a trigger (e.g., rising edge on D0). Triggers help capture the moment of interest.
- Add a decoder from the menu for common serial protocols (e.g. I2C, SPI, UART).