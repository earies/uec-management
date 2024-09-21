tree:
	@pyang \
		--strict -W error \
		-f tree \
		uec-uet-inc.yang

tests: test-00

test-00:
	@yanglint \
		-p ~/repo/github.com/openconfig/public \
		-f json \
		instance-data.json \
		uec-uet-inc.yang | jq '.'
