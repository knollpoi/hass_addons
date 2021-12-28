# Home Assistant Add-on: Dnsmasq

## Installation

Follow these steps to get the add-on installed on your system:

1. Navigate in your Home Assistant frontend to **Supervisor** -> **Add-on Store**.
2. Find the "Dnsmasq" add-on and click it.
3. Click on the "INSTALL" button.

## How to use

The add-on has a couple of options available. For more detailed instructions
see below. The basic thing to get the add-on running would be:

1. Start the add-on.

## Configuration

The Dnsmasq add-on can be tweaked to your likings. This section
describes each of the add-on configuration options.

Example add-on configuration:

```yaml
dhcp_ranges:
  - start: 10.10.10.10
    end: 10.10.10.100
    mask: 255.255.255.0
    leasetime: 24h
dhcp_options: []
vendor_options: []
```

### Option: `dhcp_ranges.start` (required)

Specifies the starting IP address of a DHCP range.

### Option: `dhcp_ranges.end` (required)

Specifies the ending IP address of a DHCP range.

#### Option: `dhcp_ranges.mask` (required)

Specifies the network mask for the range.

#### Option: `dhcp_ranges.leasetime` (required)

Specifies the lease length for addresses in this range.

## Support

Got questions?

You have several options to get them answered:

In case you've found a bug, please [open an issue on our GitHub][issue].

[issue]: https://github.com/knollpoi/hass_addons/issues
[repository]: https://github.com/knollpoi/hass_addons/tree/master/dnsmasq
