# ERC721 Vyper implementation

## Setup

`npm i`

## Testing

`npm run test`

If you make any modifications to the contracts, you will need re-compile: 

`npm run build`

A truffle compatible build process is handled by [`truper`](https://www.npmjs.com/package/truper), which does not include vyper compiler. You will need to have the `vyper` compiler installed and available in your terminal's environment. If you can't run `$ vyper -h`, the build process will fail. 

See the [Vyper installation instructions](https://vyper.readthedocs.io/en/latest/installing-vyper.html).

## TODOs

[] Remove the mint()/burn() functions. Satisfy testing requirements by 'minting' during initialization.
[] Implement the `safeTransfer()` function with data. (Dependent on adding [default parameter values in vyper](https://github.com/ethereum/vyper/issues/903))
[] Add the erc721 MetaData interface
[] Check the validity of my `onERC721Received()` function


## Acknowledgements

The test suite used here is taken from [0xCert's ethereum-erc721](https://github.com/0xcert/ethereum-erc721), with only minor modifications. Thank you to them for their work. 