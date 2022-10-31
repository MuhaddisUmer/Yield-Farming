# MyFarm Frontend
After deployment, the list of requisite addresses will be logged into your terminal. Add the addresses to the frontend/src/App.js file inside the correct load contract functions. They will look like this:
```
const loadMyFarmContract = useCallback(async(_provider) => {
    let MyFarmAddress = "0x..."
    let contract = new ethers.Contract(MyFarmAddress, MyFarm.abi,_provider)
    setMyFarmContract(contract)
    }, [setMyFarmContract])
```
***
Inside the yield-farm/frontend directory:
```
npm i
```
before finally:
```
npm run start
```
