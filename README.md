Policy
------
	iptables.policy({
		table: 'filter', // default: filter
		chain: 'FORWARD',
		target:'ACCEPT'
	}, function (error) {
		if (error) {
			console.log(error);
		}
	});

New
---
	iptables.new({
		table: 'filter', // default: filter
		chain: 'new-user-chain'
	}, function (error) {
		if (error) {
			console.log(error);
		}
	});

Rename
------
	iptables.rename({
		table: 'filter', // default: filter
		old_name: 'old-chain-name',
		new_name: 'new-chain-name'
	}, function (error) {
		if (error) {
			console.log(error);
		}
	});

Delete Chain/s
--------------
	iptables.deleteChain({
		table: 'filter', // default: filter
		chain: 'chain-name'
	}, function (error) {
		if (error) {
			console.log(error);
		}
	});

Zero
----
	iptables.zero({
		table: 'filter', // default: filter
		chain: 'chain-name',
		rulenum: 4
	}, function (error) {
		if (error) {
			console.log(error);
		}
	});

Flush
-----
	iptables.flush({
		table: 'filter', // default: filter
		chain: 'chain-name'
	}, function (error) {
		if (error) {
			console.log(error);
		}
	});